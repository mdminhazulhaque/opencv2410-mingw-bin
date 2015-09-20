# OpenCV 2.4.10 MinGW x86 Build

This is a MinGW x86 build of OpenCV 2.4.10 library. It works with Codeblocks and also with Qt 5.5 x86.

# How to Use

Assuming that, OpenCV binaries and include files are located at `C:\opencv2410`.

Add the DLLs and include files as CXX flags. For example,

    -IC:\opencv2410\include \
    -LC:\opencv2410\bin \
    -llibopencv_calib3d2410 \
    -llibopencv_contrib2410 \
    -llibopencv_core2410 \
    -llibopencv_features2d2410 \
    -llibopencv_flann2410 \
    -llibopencv_gpu2410 \
    -llibopencv_highgui2410 \
    -llibopencv_imgproc2410 \
    -llibopencv_legacy2410 \
    -llibopencv_ml2410 \
    -llibopencv_nonfree2410 \
    -llibopencv_objdetect2410 \
    -llibopencv_ocl2410 \
    -llibopencv_photo2410 \
    -llibopencv_stitching2410 \
    -llibopencv_superres2410 \
    -llibopencv_video2410 \
    -llibopencv_videostab2410

# With Qt5

A working Qt5 project file would be

    win32 {
        LIBS += -LC:\opencv2410\bin \
        -llibopencv_calib3d2410 \
        -llibopencv_contrib2410 \
        -llibopencv_core2410 \
        -llibopencv_features2d2410 \
        -llibopencv_flann2410 \
        -llibopencv_gpu2410 \
        -llibopencv_highgui2410 \
        -llibopencv_imgproc2410 \
        -llibopencv_legacy2410 \
        -llibopencv_ml2410 \
        -llibopencv_nonfree2410 \
        -llibopencv_objdetect2410 \
        -llibopencv_ocl2410 \
        -llibopencv_photo2410 \
        -llibopencv_stitching2410 \
        -llibopencv_superres2410 \
        -llibopencv_video2410 \
        -llibopencv_videostab2410
        INCLUDEPATH += C:\opencv2410\include
    }

# FFMPEG

FFMPEG support has been tested using x264 encoded video. `opencv_ffmpeg2410.dll` has been included inside `bin` directory.
