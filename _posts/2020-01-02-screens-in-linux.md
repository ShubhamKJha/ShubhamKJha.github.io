---
layout: post
title: screen command in Linux
comments: true
tags: [linux]
categories: [dev experiences]
---

<div style="text-align: left;">
It happens to computer enthusiasts that they encounter certain things during working on something else. I happen to work on many different things in the last few days and did encounter a great deal of hidden treasures. I hope I could have found them earlier. Like any treasure hunter I would like to show off my findings. So, carry along.</div>
<br />
The first one would certainly be the <b>screen</b> command in Linux.<br />
<br />
Linux lovers would understand my love for it's terminal. Although I have personally been a fan of latest Windows' UI yet even the recent developments in Command-Prompt doesn't incite a same liking in me. I am a fan of doing everything on key-board (unless not possible). The power of Linux terminal always gets me back into it and whenever I think I know enough, there is always something that gets me hooked again. Recently, during a course on Coursera, its instructor pointed out the necessity of having a terminal instance running in the background. A server was connected using <b>ssh</b> and a certain program has to be run in the background even after the ssh-session ends. It was calmly done using the <b>screen </b>command. And yes it is one of the use-cases of this command.<br />
<h3 style="text-align: left;">
&nbsp;</h3>
<h3 style="text-align: left;">
Get to know it!</h3>
The <b>screen </b>command<b> </b>lets a user to open several terminal instances inside one single terminal window manager. The other sessions keep running in the background and are detached when not required. These can later be reattached and they keep running as they are. It gives the effect of running several terminals but unlike several terminals, they keep running even when the main terminal window is closed.<br />
<br />
Advantages:<br />
<ul style="text-align: left;">
<li>You can detach the screens you are not working on. This way your terminal wouldn't be filled with unwanted details about installations, downloads, etc.</li>
<li>You can reattach to those screens without losing anything. The screens would be running as if nothing happened.</li>
<li>You can work on different things in different screens without opening new terminals. </li>
</ul>
<h3 style="text-align: left;">
&nbsp;</h3>
<h3 style="text-align: left;">
Installing screen</h3>
On Debian-based systems:<br />
<blockquote class="tr_bq">
<span style="background-color: #f3f3f3;"><code>
</code></span><b><span style="font-family: &quot;courier new&quot; , &quot;courier&quot; , monospace;">$ sudo apt-get install screen </span></b></blockquote>
<br />
<code></code>On RedHat based systems:<br />
<blockquote class="tr_bq">
<code>
</code><b><span style="font-family: &quot;courier new&quot; , &quot;courier&quot; , monospace;">$ yum install screen</span></b></blockquote>
<h3 style="text-align: left;">
</h3>
<h3 style="text-align: left;">
&nbsp;</h3>
<h3 style="text-align: left;">
Using screen</h3>
<ul style="text-align: left;">
<li>Screens can be created using</li>
</ul>
<blockquote class="tr_bq">
<b><span style="font-family: &quot;courier new&quot; , &quot;courier&quot; , monospace;">$ screen -S &lt;screen-name&gt;</span></b></blockquote>
<ul style="text-align: left;">
<li>List all the screen</li>
</ul>
<blockquote class="tr_bq">
&nbsp;<b><span style="font-family: &quot;courier new&quot; , &quot;courier&quot; , monospace;">$ screen -ls</span></b></blockquote>
<ul style="text-align: left;">
<li>Switch (reattach) to a particular screen&nbsp;</li>
</ul>
<blockquote class="tr_bq">
<b><span style="font-family: &quot;courier new&quot; , &quot;courier&quot; , monospace;">$ screen -r &lt;screen-name&gt;</span></b></blockquote>
<ul style="text-align: left;">
<li>Detach from a screen (to the main terminal)</li>
</ul>
<blockquote class="tr_bq">
<span style="font-family: &quot;courier new&quot; , &quot;courier&quot; , monospace;"><b>CTRL-A + CTRL-D</b></span></blockquote>
<ul style="text-align: left;">
<li>To close a screen</li>
</ul>
<blockquote class="tr_bq">
<span style="font-family: &quot;courier new&quot; , &quot;courier&quot; , monospace;"><b>CTRL-D</b></span> </blockquote>
<ul style="text-align: left;">
<li>You can also password-protect your screens simply use <b><span style="font-family: &quot;courier new&quot; , &quot;courier&quot; , monospace;">CTRL-X</span> </b>from within your screen. And only it can be opened using the password of your PC. </li>
</ul>
<div style="text-align: left;">
<br /></div>
<br />
I won't go into much details here (even I have just started using it). For more understanding you can always <b>Google </b>more, or use <span style="font-family: &quot;courier new&quot; , &quot;courier&quot; , monospace;">man(screen)</span>to learn more about it.<br />
&nbsp; <br />
<div>
<div>
<div>
The following is an&nbsp;<a href="https://asciinema.org/">asciinema</a> (another good project I got to know recently) showing some working of <b>screen</b> command. <br />
<br />
<script async="" id="asciicast-Gn5e3KJBABI57yYyQ1WyQyJx6" src="https://asciinema.org/a/Gn5e3KJBABI57yYyQ1WyQyJx6.js"></script> </div>
</div>
I hope this gave some insights into using a good tool.<br />
<br /></div>