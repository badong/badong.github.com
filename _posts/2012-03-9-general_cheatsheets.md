---
layout: post
title: general cheatsheets
---

<p class="meta">09 March 2012 - San Francisco</p>
1. `127.0.0.1` Is the default IP address for `localhost`
2.  `public void printf(String s, Object...args)` the 3 dots is call varargs. It means you can pass 0 or more arguments. 
Its a shortcut to creating array manually
3. Convert integer to binary representation
{% highlight java %}
for(int i=0; i<32; i++)
sum+=( num >> i ) & 1;
System.out.println( sum );
{% endhighlight %}
OR
{% highlight ruby %}
for(int i=0; i<32; i++)
  cout<<(n<0)      //shift left, then check (n<0? '1' : '0')
 	n*=2;
{% endhighlight %}
4. View if port is running a process `lsof -w -n -i tcp:8888` then you can kill the port by doing `kill [pid]`

                        







