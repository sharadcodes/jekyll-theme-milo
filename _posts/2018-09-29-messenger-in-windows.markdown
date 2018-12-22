---
title: Messenger in Windows
date: 2018-09-29 10:25:00 Z
layout: post
categories:
- WINDOWS
- SCI-TECH
---

<p class="intro">
<span class="dropcap">H</span>i ! there I am back again with another interesting geeky thing for you. Today we will create our own simple CMD based messenger for chatting with anyone on another PC. So lets get started.
</p>

### REQUIREMENTS

1. Windows PC.

2. Any Text Editor ( Notepad, Notepad\+\+, Sublime etc).

3. IP Address of the PC of person you want to chat.

4. Internet Connection.

### LETS BEGIN

1. Open Notepad or any other text editor.

2. Open a **new file**  and **paste** the code below in it.

{% highlight bash %}
@ echo off
\:A
Cls
echo MESSENGER
set /p n=User:
set /p m=Message:
net send %n% %m%
Pause
Goto A
{% endhighlight %}

Save the file on Desktop with name **messenger.bat** and Close it.

So now you have finished making your own messenger in Windows. So quickly call your friend and ask for his IP .

If you don’t know what is your IP open CMD and type ipconfig and press enter key.

You will see the **IPv4 address** **Note it that’s your IP.**

### HOW TO USE MESSENGER

Just double click on file and enter your friend’s IP address in **USER** and press enter and the text in **MESSAGE** and press enter.

### Thank you !