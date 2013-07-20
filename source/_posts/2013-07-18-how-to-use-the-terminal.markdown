---
layout: post
title: "how to use the terminal"
date: 2013-07-18 20:42
comments: true
categories: ["Terminal", "Commands", "Files", "Folders", "Directories", "Unix", "DOS", "Shell", "ITerm"]
---

Hey Maddie! Welcome to your first tutorial. Today you'll learn what a terminal is and how to use it. Simply, a terminal is where you enter commands that directly deal with a computer. It can be used to tell which files are in a folder, move files, rename files and folders, browse files and see what's in them, and so much more. By the way when you're using a terminal you call **"folders", "directories"**. Programmers prefer terminals over your everyday windows because they're faster and more flexible with the ways you interact with a computer. Also without terminals there would be a significant decrease in performance of programs running on your computer. There are several different types of terminals. The most important difference between them is the operating system that uses it. For example Windows has their own special kind of terminal called DOS. While most other major operating system such as Mac OSX and Linux uses a UNIX based terminal that many people refer to as a Shell. Our primary focus will be on the UNIX Shell or for our purpose we'll just call it terminal.  

Before we can start using the terminal you have to know how to open it. I like to do it the fast way by holding Command and pressing space. When you do this you'll see a blue and white search bar appear at the top right of your screen that says "Spotlight". When you see this, type ITerm and press enter. If that doesn't work you can just click on "Finder" and go to **Applications > ITerm.**  
Either way you do it, you should see a window that pops up that looks something like this:  
{% img /images/iterm-open.png %}  
Right now you're in your "home" folder or as we call it your "home" directory. Test it out by typing:
{% codeblock lang:bash %}
echo hello
{% endcodeblock %}  
and press enter.  
If you did this correctly you should see "hello" was outputted below the line you just typed. You just entered your first command! A command consists of a name (in this case "echo") and 0 or more arguments (in this case "hello" being the only argument). As you can tell all the "echo" command does is, well, echo whatever it's arguments are. Always remember that a command won't execute or run until your press enter on your keyboard. Since this is your first day we're just going to mess around with the most frequently used commands. The ones I'll be teaching today are 'ls', 'cd', and 'mkdir'. Let's start with ls by simply typing:
{% codeblock lang:bash %}
ls
{% endcodeblock %}
You should see a bunch of things that were output such as "Downloads", "Movies", "Music", "Documents", and most likely some other stuff. the "ls" command in this case taking 0 arguments simply shows all of the files and folders in a directory. It's purpose is to show what files and folders exist in a directory. That's kind of useful! And now let's use "cd". No, it has nothing to do with CD's that contain music lol. "cd" is short for change directory. let's "change directory" to "Downloads" by typing:
{% codeblock lang:bash %}
cd Downloads
{% endcodeblock %}
At this point you should be in the Downloads directory. This is where all the files you have downloaded are stored and remember you can see all these files by typing:
{% codeblock lang:bash %}
ls
{% endcodeblock %}
So the "cd" command takes 1 argument. This argument should be the directory that you want to go in to and in our case that 1 argument was "Downloads".
To go back to the home directory simply type:
{% codeblock %}
cd ../
{% endcodeblock %}
The "../" argument to "cd" takes you back one directory.  
And finally, for today, is the "mkdir" command. This is responsible for creating a new directory. This is just like creating a new folder by right-clicking on the finder window and selecting the "Create a new folder" option. Let's just create a directory called "favs" for purposed of demonstration. You can do this by typing:
{% codeblock lang:bash %}
mkdir favs
{% endcodeblock %}
You can use this folder to put all your favorite stuff in. If that's what you want to do. As you can see the "mkdir" command took 1 argument that specifies the name of the new directory that you want to create and in this situation we created a new directory named "favs". We verify that by using the "ls" command and seeing the output of that contains "favs". If you want you can even go inside your newly created directory by typing:
{% codeblock %}
cd favs
{% endcodeblock %}
However it shouldn't be too surprising that a new directory won't have anything inside of it yet. You can once again verify that by typing:
{% codeblock %}
ls
{% endcodeblock %}
Which shows all files and folders in that directory (this time nothing will show up).  

Get ready for the next post where I show you how to delete files and folders, create new files, and show what's inside of a file. All by using a terminal Thanks for reading. Hope to see you on here soon!