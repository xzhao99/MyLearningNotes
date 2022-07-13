_________________________________
## Scientific Computing Libraries:
* [Petsc](https://petsc.org/)
* [Trilinos](https://trilinos.github.io/)
* [Slepc](https://slepc.upv.es/)
* [Boost](https://www.boost.org/)
* [Eigen](https://eigen.tuxfamily.org/)
* [spectra](https://spectralib.org/): C++ Library For Large Scale Eigenvalue Problems(built on top of Eigen)

_________________________________

## Finite Element Libraries:
* [deal.II](https://www.dealii.org): C++ based finite element simulation package
* [deal2lkit](https://github.com/mathLab/deal2lkit): A ToolKit library for deal.II
* [PRISMS-PF](http://prisms-center.github.io/phaseField/): An open-source, general purpose framework for high-performance phase field modeling(using deal.II by UMich)
  This will give a good example on how to build your own applications on top of deal.II using CMake:
  https://prisms-center.github.io/phaseField/doxygen_files/install.html
* [libMesh](https://libmesh.github.io/): adaptive finite element library
* [MOOSE](https://mooseframework.inl.gov/): Multiphysics Object-Oriented Simulation Environment finite element framework, built on top of libMesh and PETSc
* [FEniCS](https://fenicsproject.org/) Python based finite element simulation package
* [MFEM](https://mfem.org/): Parallel FEM library developed in LLNL supporting higher-order FE, IGA, DG, Mixed FE, Mesh optimization, CPU/GPU parallelization and many other features.
* [BACI](https://baci.pages.gitlab.lrz.de/website/index.html): A Comprehensive Multi-Physics Simulation Framework(Prof. Dr.-Ing. Wolfgang A. Wall in TUM, not open-source)
_________________________________

## IGA
* [IGA-dealii](https://github.com/mathLab/IGA-dealii): Isogeometric Analysis classes for the deal.II library
* [G+Smo](https://gismo.github.io/):
G+Smo (Geometry + Simulation Modules, pronounced "gismo") is an open-source C++ library that brings together mathematical tools for geometric design and numerical simulation. It implements the relatively new paradigm of isogeometric analysis, which suggests the use of a unified framework in the design and analysis pipeline. G+Smo is an object-oriented, cross-platform, template C++ library and follows the generic programming principle, with a focus on both efficiency and ease of use. The library aims at providing access to high quality, open-source software to the forming isogeometric numerical simulation community and beyond.

_________________________________

## Geometry
* Computatianl Geometry and Mesh Processing:
  * [CGAL](https://www.cgal.org/)
  * [libigl](https://libigl.github.io/): a simple header-only C++ geometry processing library.
  * [PMP: Polygon Mesh Processing Library](https://www.pmp-library.org/)
  * [VCGLib](https://github.com/cnr-isti-vclab/vcglib), [Documentation](http://vcg.isti.cnr.it/vcglib/)
  * [MeshLab](https://github.com/cnr-isti-vclab/meshlab) (use VCGLib as the kernel)
  * [OpenMesh](www.openmesh.org)
  * [OpenFlipper](https://www.openflipper.org/): A multi-platform application using OpenMesh
  * [Cinolib](https://github.com/mlivesu/cinolib): a C++ library for processing polygonal and polyhedral meshes (MIT license) by [Marco Livesu](http://pers.ge.imati.cnr.it/livesu/)
  * Mesh Denoising code in Github:
    - [Guided Mesh Denoising](https://github.com/bldeng/GuidedDenoising/tree/master/src): Open-source code for mesh denoising algorithms
    - [Mesh total generalized variation for denoising](https://github.com/LabZhengLiu/MeshTGV)
  * [libQEx](https://github.com/hcebke/libQEx) – A Robust Quad Mesh Extractor(source code in github)
* CAD:
  * [OpenCascade](https://dev.opencascade.org/)
* Mesh Generation:
  * [Gmsh](https://gmsh.info/)
  * [TetGen](https://wias-berlin.de/software/index.jsp?id=TetGen)
    * [a course on Mesh Generation Methods and Softwares](https://www.wias-berlin.de/people/si/?lang=1)
  * [TetWild](https://github.com/Yixin-Hu/TetWild) and [fTetWild](https://github.com/wildmeshing/fTetWild) - (Fast) Tetrahedral Meshing in the Wild
  * [TriWild: Robust Triangulation With Curve Constraints](https://github.com/wildmeshing/TriWild)
* Visualization and Rendering:
  * [VTK](https://vtk.org/)
  * [ITK](itk.org)
  * [ParaView](https://www.paraview.org/)
  * [VisIt](https://visit-dav.github.io/visit-website/)
  * [Blender](https://www.blender.org/)
* CG Tools and solvers:
  * [OpenVDB](https://www.openvdb.org/): open-source C++ library of sparse volumetric data discretized on three-dimensional grids
  * [Surface Multigrid via Intrinsic Prolongation](https://github.com/HTDerekLiu/surface_multigrid_code): geometric multigrid solver on top of libigl
* Point Clouds:
  * [CloudCompare](https://www.cloudcompare.org/main.html)
  * [Point Cloud Library (PCL)](https://pointclouds.org/)
  * [3DKT](https://slam6d.sourceforge.io/): 
  * [Awesome-Point-Cloud-Processing](https://github.com/mmolero/awesome-point-cloud-processing): A curated list of awesome Point Cloud Processing Resources, Libraries, Software.

### Tutorials and Learning materials:
  * [A Gentle Introduction to **Bilateral Filtering** and its Applications](https://people.csail.mit.edu/sparis/bf_course/):
    - Tutorial/Course notes, slides and code tought at ACM SIGGRAPH 2007,2008/IEEE CVPR 2008
    - Related course links of Computational photography and Level set for computer graphics

_________________________________

## Computer vision:
* [openMVG](https://github.com/openMVG/openMVG): open Multiple View Geometry
* [AliceVision](https://github.com/alicevision/AliceVision): a Photogrammetric Computer Vision Framework which provides a 3D Reconstruction and Camera Tracking algorithms. 

_________________________________

## Dev
* [Intel ONEAPI Toolkits](https://www.intel.com/content/www/us/en/developer/tools/oneapi/overview.html#gs.0ia0ni)
* [CLI11](https://github.com/CLIUtils/CLI11): CLI11: Command line parser for C++11.
* [BOOST.Log](https://github.com/boostorg/log): part of collection of the Boost C++ Libraries, provides tools for adding logging to libraries and applications.
* [plog](https://github.com/SergiusTheBest/plog) - portable, simple and extensible C++ logging library
* [glog](https://github.com/google/glog): C++ implementation of the Google logging module
* [GoogleTest](https://github.com/google/googletest): Google Testing and Mocking Framework [User's Guide](https://google.github.io/googletest/)
* [GoogleBenchmark](https://github.com/google/benchmark)
* [Catch2](https://github.com/catchorg/Catch2)
  * [Official doc on CMake integration](https://github.com/catchorg/Catch2/blob/devel/docs/cmake-integration.md)
  * [Integration with CMake/CTest in StackOverflow](https://stackoverflow.com/questions/34896891/catch-lib-unit-testing-and-ctest-cmake-integration)
  * [CMake example in Github](https://github.com/ComicSansMS/GhulbusBase/blob/master/CMakeLists.txt)
* [Best Open Source CI/CD tools for 2022](https://hevodata.com/learn/open-source-ci-cd-tools/)
  * [Jenkins](https://www.jenkins.io/): a CI/CD platform for auto build, test and deploy code.
  * Gradle
  * GitLab
  * CodeShip
  * Buddy
  * GoCD
  * CTest/CDash: [Tutorial](https://embeddeduse.com/2022/05/02/building-a-ci-pipeline-with-ctest-and-cdash/)

_________________________________

## Cross-Platform Package Management:
* [Anaconda](https://anaconda.org/)
  - [miniconda](https://docs.conda.io/en/latest/miniconda.html)
  - [Conda-forge](https://conda-forge.org/)
  - [Conda-user guide](https://docs.conda.io/projects/conda/en/latest/user-guide/index.html)
  - [RHEL7 ANACONDA CUSTOMIZATION GUIDE](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html-single/anaconda_customization_guide/index#sect-anaconda-visuals-graphics)
* [Mamba](https://github.com/mamba-org/mamba)
* [vcpkg](https://github.com/microsoft/vcpkg)
  - [vcpkg — C++ Easy Mode Step by Step Tutorial](https://gamefromscratch.com/vcpkg-cpp-easy-mode-step-by-step-tutorial/)
  - [YouTube resources](https://www.youtube.com/results?search_query=vcpkg)
* [conan](https://conan.io/)
* conan vs vcpkg:
  - [Vcpkg Vs Conan: Best Package Manager For C++?](https://matgomes.com/vcpkg-vs-conan-for-cpp/)
  - [vcpkg-vs-conan: features comparison](https://github.com/52doho/vcpkg-vs-conan)

### Reference:
* [C++ Development With Conda](https://www.prouvost.dev/post/2021/c-development-with-conda)
* 

### Applied Mathematics Laboratory @ SISSA:
* https://mathlab.sissa.it/
* https://github.com/mathLab

_________________________________
