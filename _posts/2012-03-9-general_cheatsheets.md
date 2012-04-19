---
layout: post
title: general cheatsheets
---

<p class="meta">09 March 2012 - San Francisco</p>
1. `127.0.0.1` Is the default IP address for `localhost`
2.  `public void printf(String s, Object...args)` the 3 dots is call varargs. It means you can pass 0 or more arguments. 
Its a shortcut to creating array manually
3. `et.setInputType(InputType.TYPE_CLASS_PHONE);`  `et.setInputType(InputType.TYPE_CLASS_TEXT)` 
Set the input type for EditText
4. `<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />` - add this to androidManifext.xml if 
    you want to write file in /sdcard in android SD card 
5. Convert integer to binary representation
`for(int i=0; i<32; i++)`
` sum+=( num >> i ) & 1;`
`System.out.println( sum );`
6. View if port is running a process `lsof -w -n -i tcp:8888` then you can kill the port by doing `kill [pid]`
7. `adb shell top -m 10` - to view the CPU process for android device. Make sure device is connected to PC
                        







