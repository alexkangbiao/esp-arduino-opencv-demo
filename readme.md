# Arduino use openCV on ESP32

1. Copy Opencv Lib to ./lib
2. add to platformio.ini
```ini
lib_deps = 
    opencv
build_flags =
    -L ./lib/opencv
    -llibopencv_imgproc.a
    -llibopencv_core.a
```
3. add partitions for opencv static library
```shell
  816k libade.a
 8618k libopencv_core.a
  498k libopencv_imgcodecs.a
 8277k libopencv_imgproc.a
```

## GITHUB
```shell
git config --global user.email "you@example.com"
  git config --global user.name "Your Name"
  git init
  git add README.md
  git commit -m "first commit"
  git branch -M main
  git remote add origin https://github.com/alexkangbiao/esp-arduino-opencv-demo.git
  git push -u origin main

```