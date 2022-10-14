# Pro tip:
To solve this error:
````
(mach-o file, but is an incompatible architecture (have 'arm64', need 'x86_64'))
```
In order for Azure Functions with python to work on a Mac M1 this dependencys need to be installed in a x86_64 architecture
```
arch -x86_64 pip3 install numpy
arch -x86_64 pip3 install opencv-python
arch -x86_64 pip3 install onnxruntime
```
