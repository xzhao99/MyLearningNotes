cmake - handling executable and library with same name
CMakeLists.txt

Lets say we want to add a library and an executable, both with the same name. 
In this example, it is resman
```
add_library(resman ${src_cpps} ${src_hpps} )
target_link_libraries(resman ${Boost_LIBRARIES} ${LIBYAML} ${LIBFMT})
```
Add resman executable

We call the executable resman-bin
```
add_executable(resman-bin main.cpp ) 
target_link_libraries(resman-bin resman)
```

now we rename resman-bin executable to resman using target properties
```
set_target_properties(resman-bin
        PROPERTIES OUTPUT_NAME resman)
```

https://gist.github.com/jlgerber/eafc4ee2b9954e27dd2bb009496b1b03
