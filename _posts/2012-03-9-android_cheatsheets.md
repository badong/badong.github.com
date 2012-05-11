---
layout: post
title: Android cheatsheets
---

<p class="meta">09 March 2012 - San Francisco</p>
1.  `adb shell top -m 10` - to view the CPU process for android device. Make sure device is connected to PC
2.  `et.setInputType(InputType.TYPE_CLASS_PHONE);`  `et.setInputType(InputType.TYPE_CLASS_TEXT)` 
Set the input type for EditText
3. `<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />` - add this to androidManifext.xml if 
    you want to write file in /sdcard in android SD card
4. When you are calling a startActivity() outside of an activity. i.e.you are calling it in a superclass you should add this `in.addFlags(Intent.FLAG_ACTIVITY_NEW_TASK);`
{% highlight java %}
Intent in = new Intent("TESTGOTOCHAT");
//need this code if calling startActivity is called outside of an Activity
in.addFlags(Intent.FLAG_ACTIVITY_NEW_TASK);
Bundle b= new Bundle();
b.putString("name", userName );
in.putExtras(b);
mContext.getApplicationContext().startActivity(in);
{% endhighlight %}







