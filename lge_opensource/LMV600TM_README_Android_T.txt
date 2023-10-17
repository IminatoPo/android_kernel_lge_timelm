1. Android build
  - Download original android source code ( android-13.0.0_r11) from http://source.android.com   
  ( $repo init -u https://android.googlesource.com/platform/manifest -b android-13.0.0_r11
    $repo sync -cdq -j12 --no-tags
    $repo start android-13.0.0_r11 --all 
  )
  - And, merge the source into the android source code
  
  - Run following scripts to build android
    a) source build/envsetup.sh
    b) lunch 1
    c) make -j4
  - When you compile the android source code, you have to add google original prebuilt source(toolchain) into the android directory.
  - After build, you can find output at out/target/product/generic

2. to obtain the open data about KnowMeABBA*.apk App  

 If you want to obtain the open data ( source ) for "KnowMeABBA or *ABBA.apk " application, 
 the open data may be obtained at http://opensource.lge.com. 
 LGE will also provide open data ( code ) to you . 
 
 You can search the keyword with "KnowMeABBA" at the search window in http://opensource.lge.com.  

 You can find it in "Software List" at that website.

