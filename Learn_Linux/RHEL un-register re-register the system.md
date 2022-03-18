Execute the following steps in exactly the given order. :)

Un-register the system :
```
sudo subscription-manager remove --all
sudo subscription-manager unregister
sudo subscription-manager clean
```
Re-register the system :
```
sudo subscription-manager register
sudo subscription-manager refresh
```
Search for the Pool ID :
```
sudo subscription-manager list --available
```
Attach to subscription :
```
sudo subscription-manager attach --pool=<Pool-ID>
```
Clean YUM and cache :
```
sudo yum clean all
sudo rm -r /var/cache/yum
```
Update the resources :
```
sudo yum upgrade
```
