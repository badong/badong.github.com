---
layout: post
title: java tips
---

<p class="meta">07 March 2012 - San Francisco</p>
1. In Java,when creating threads, it shares a copy of the instance variable. example below

<script src="https://gist.github.com/1988822.js"> </script>

2. In Java, you need to lock or synchroniz the variable that is being used by two or more threads to prevent deadlock

3. When your program is modifying String all the time (example game logic, operations, construction of string) then you need 
to use StringBuilder or StringBuffer. String Object is immutable so whenever you alter the value, another object is created
so memory allocation needs to occur. You don't want that to happen in a game loop where you allocate memory every loop. This 
will cause GC to run every now and then.

* Use StringBuilder if only one thread is accessing it
* Use StringBuffer if one or more thread is accessing it, StringBuffer is thread-safe






