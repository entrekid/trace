# System settings for DL in OSX

* For using nvidia cards on OSX is really hard stuff, those are working settings on my MBP16(19').

* I really care 'bout egpu.io(the coolest community for egpu users), but not many tutorials worked on my system(actually almost broke it..)

* The new gpu users(as RTX 30 series) should be care for # of pins. My system didn't detect any of my machines so at first I just concerned about my os kernels but lots of my tries gonna failed.(e.g : dockerizing, vmware, managing my boot-loader using efi-bootloader. but none of these worked : but I heard lots of successful cases using machines under 20 series)

* And always remember making virtual environment time machine both of your os and for frameworks. 


* Tensorflow version should be nightly.(12/28 worked)

* Tensorflow now works(pip install tensorflow)

* pytorck now works(In my case, conda packaging not worked, so I recommend using pip install) (pip install torch===1.7.1+cu110 torchvision===0.8.2+cu110 torchaudio===0.7.2 -f https://download.pytorch.org/whl/torch_stable.html)
