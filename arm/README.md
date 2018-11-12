# Bypass Facebook Messenger SSL Pinning (REQUIRE ROOTED)
Bypassing Facebook Messenger SSL pinning for version 188.0.0.33.100 | arm | November 1, 2018
[Download Link](https://www.apkmirror.com/apk/facebook-2/messenger/messenger-148-0-0-20-381-release/facebook-messenger-148-0-0-20-381-android-apk-download/)


#### libcoldstart.so

Replace the libcoldstart.so file in **/data/data/com.facebook.orca/lib-xzs**



## Steps:



We need to patch **0x0025B24C** and **0x0025B24E**:

![before_patching](https://raw.githubusercontent.com/knoobdev/Bypass-Facebook-Messenger-SSL-Pinning/master/arm/before_patch.jpg?54119)


After patching these offsets to **0xB1C4** and **0xB948**, patched lib should be like this:


![after_patching](https://raw.githubusercontent.com/knoobdev/Bypass-Facebook-Messenger-SSL-Pinning/master/arm/after_patch.jpg?54119)

---



[Refrence](https://serializethoughts.com/2016/08/18/bypassing-ssl-pinning-in-android-applications/) & Thanks for [pouyadarabi](https://github.com/pouyadarabi/Facebook_SSL_Pinning)

