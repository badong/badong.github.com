---
layout: post
title: general cheatsheets
---

<p class="meta">09 March 2012 - San Francisco</p>
1. `127.0.0.1` Is the default IP address for `localhost`

2.  `public void printf(String s, Object...args)` the 3 dots is call varargs. It means you can pass 0 or more arguments. 
Its a shortcut to creating array manually

3. **Convert integer to binary representation**
{% highlight java %}
//note this goes from 31 to 0, so it will loop 32 times
for(int i=31; i>=0; i--)
{
sum=( num >> i ) & 1;
System.out.println( sum );
}
{% endhighlight %}
OR
{% highlight ruby %}
for(int i=0; i<32; i++)
{      
	System.out.print(n<0 ? '1' : '0');  //shift left, then check (n<0? '1' : '0')
 	n*=2;
}//this will cause overflow 
{% endhighlight %}

**Binary to Integer
{% highlight java %}
    int n=111;
    int sum=0;
    for(int i=0; i<32; i++)
    {
       int mod = n%10;
       if(mod==1)
          sum+= Math.pow(2, i);
       n= n /10;           
    }
    System.out.println(sum);
{% endhighlight %}
4.View if port is running a process `lsof -w -n -i tcp:8888` then you can kill the port by doing `kill [pid]`

5.**Remove three larges int in an array function**

{% highlight java %}
//@param array and size of array
void reduce(int a[], in& n)
{
	int i, j, k=3, max;
	while(k--)
	{
		//find maximum
		for(max=a[0]; i=1; i<n; i++)
			if(a[i] > max) max=a[i];
	
		//eliminate the duplicate
		for(j=i=0; i<n; i++)
			if(a[i]!=max) a[j++]=a[i]	//moving j++ only when a[i] is not equal to max
	
	//changing the size of array to new size
	n=j;
	}
}
{% endhighlight %}

6.The use of carat ^. This is use if you want to flip something. i.e. use in turn base. 
{% highlight java %}
//0 means player1 turn, 1 means player 2 turns
int turn=0;
turn = turn ^ 1;	//this will flip the value of turn
{% endhighlight %}


7.echo 'export PATH=/usr/local/mysql/bin:$PATH' >> ~/.profile

8. Absolute Path function Hack
http://www.geeksforgeeks.org/archives/2648
{% highlight java %}
int n=-2;
int mask = n>>31;
n =(mask + n) ^ mask;
System.out.println(n);
{% endhighlight %}







                        







