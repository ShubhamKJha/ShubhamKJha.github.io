---
layout: post
title: screen command in Linux
comments: true
tags: [linux]
categories: [dev experiences]
---
It happens to computer enthusiasts that they encounter certain things during working on something else. I happen to work on many different things in the last few days and did encounter a great deal of hidden treasures. I hope I could have found them earlier. Like any treasure hunter I would like to show off my findings. So, carry along.

The first one would certainly be the **screen** command in Linux.

Linux lovers would understand my love for it's terminal. Although I have personally been a fan of latest Windows' UI yet even the recent developments in Command-Prompt doesn't incite a same liking in me. I am a fan of doing everything on key-board (unless not possible). The power of Linux terminal always gets me back into it and whenever I think I know enough, there is always something that gets me hooked again. Recently, during a course on Coursera, its instructor pointed out the necessity of having a terminal instance running in the background. A server was connected using **ssh** and a certain program has to be run in the background even after the ssh-session ends. It was calmly done using the **screen** command. And yes it is one of the use-cases of this command.

#### Get to know it!
The **screen** command lets a user to open several terminal instances inside one single terminal window manager. The other sessions keep running in the background and are detached when not required. These can later be reattached and they keep running as they are. It gives the effect of running several terminals but unlike several terminals, they keep running even when the main terminal window is closed.
##### Advantages:
<ul style="text-align: left;">
  <li>You can detach the screens you are not working on. This way your terminal wouldn't be filled with unwanted details about installations, downloads, etc.</li>
  <li>You can reattach to those screens without losing anything. The screens would be running as if nothing happened.</li>
  <li>You can work on different things in different screens without opening new terminals. </li>
</ul>


#### Installing screen
On Debian-based systems:
```bash
$ sudo apt-get install screen 
```
On RedHat based systems:
```bash
$ yum install screen
```

#### Using screen

* Screen can be created using
    ```bash
    $ screen -S <screen-name>;
    ```

* List all the screns.
    ```bash
    $ screen -ls;
    ```
* Switch (reattach) to a particular screen 
    ```bash
    $ screen -r <screen-name>;
    ```
* Detach from a screen (to the main terminal) 
    ```
    CTRL-A + CTRL-D
    ```
* To close a screen
    ```
    CTRL-D
    ```
* You can also password-protect your screens simply use **CTRL-X** from within your screen. And only it can be opened using the password of your PC.

I won't go into much details here (even I have just started using it). For more understanding you can always **Google** more, or use `man screen` to learn more about it.
The following is an [asciinema](https://asciinema.org) (another good project I got to know recently) showing some working of **screen** command.
<br />
<script async="" id="asciicast-Gn5e3KJBABI57yYyQ1WyQyJx6" src="https://asciinema.org/a/Gn5e3KJBABI57yYyQ1WyQyJx6.js"></script><br />
I hope this gave some insights into using a good tool.<br />