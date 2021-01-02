# System settings for DL in OSX

* For using nvidia cards on OSX is really hard stuff, those are working settings on my MBP16(19').

* I really care 'bout egpu.io(the coolest community for egpu users), but not many tutorials worked on my system(actually almost broke it..)

* The new gpu users(as RTX 30 series) should be care for # of pins. My system didn't detect any of my machines so at first I just concerned about my os kernels but lots of tries gonna failed.(e.g : dockerizing, vmware, managing my boot-loader using efi-bootloader. but none of these worked : but I heard lots of successful cases using machines under 20 series)

* And always remember making virtual environment or time machine both of your os and for frameworks. 

* Virtual environment should locate on python==3.8(cuz there are no matched version of tensorflow if using version 3.9 of python)

* Tensorflow version should be nightly.(12/28 worked --> Stable version also worked.)

* Tensorflow now works(pip install tensorflow)

* pytorch now works(In my case, conda packaging not worked, so I recommend using pip install) (pip install torch===1.7.1+cu110 torchvision===0.8.2+cu110 torchaudio===0.7.2 -f https://download.pytorch.org/whl/torch_stable.html)

* There are header issues when you use tensorflow or torch using latest anaconda versions(as in numpy 1.19.4)
Should delete that of version(pip uninstall numpy) and reinstall 1.19.3(pip install numpy==1.19.3).

* Lightgbm-gpu version install : mingw64, cmake, microsoft visual studio tools
