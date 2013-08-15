---
layout: post
title: "How to Use the Terminal (Part 3)"
date: 2013-08-01 14:01
comments: true
categories: ["Terminal", "Commands", "Files", "Folders", "Directories"]
---

Welcome! After reading the [first](/blog/2013/07/18/how-to-use-the-terminal/) and [second](/blog/2013/07/20/how-to-use-the-terminal-part-2/) tutorials you should already know what a command is, its arguments, and options. You've learned several commands so far. This post will be your final tutorial on how to use the terminal. In this post you'll learn a few more essential commands.  

##Renaming files and directories
Renaming files and directories is easy. The syntax of renaming a directory is the same as that of renaming of file and looks like this:
{% codeblock lang:bash %}
mv foo bar
{% endcodeblock %}
As you can see the name of the command we're using here is "mv" and it has 2 arguments, the file (or directory) to be renamed and the new name for that file (or directory) respectively.  

Here's what is happening:
Say we have a file with the name "foo"...  
{% img /images/foo-for-mv.png %}  
Now we want to rename that "foo" file to "bar"  
So we issue an "mv" command with "foo" as the first argument and "bar" as the second argument. Again Like this:
{% codeblock lang:bash %}
mv foo bar
{% endcodeblock %}
After executing this command, you can see that the "foo" file has been renamed to "bar" by using "ls" to see all the files in the current directory:  
{% img /images/bar-for-mv.png %}  
Keep in mind that this works for renaming directories as well. This syntax is the same for files and directories.
That's all there is to renaming things!  

##Copying files
Copying files has the same syntax as renaming files. The one exception is that the second argument is the name of the file you want to copy the first argument to.
{% codeblock lang:bash %}
cp foo bar
{% endcodeblock %}
This is saying copy the the file named "foo" to a newly created file named "bar". Note that the first and second arguments should not be the same. This is because 2 or more files in the same directory CANNOT have the same name.  
Before issuing the "cp" command you would see something like this:
{% img /images/foo-for-mv.png %}
See the file named "foo"?
After executing the "cp" command you should see something like this:
{% img /images/bar-for-cp.png %}
Notice how "foo" and "bar" are there. This is because you copied "foo" into "bar". Essentially this means you have 2 copies of "foo" but with the other file named as "bar".  

##Copying directories
Remember the "rm" command for directories? You would have to say:
{% codeblock lang:bash %}
rm -rf somedirectory
{% endcodeblock %}
Remembering the "-rf" option to "rm", this should have removed the directory. However not remembering it, the terminal would complain that "somedirectory" is a directory and that you cannot remove a directory without the "-rf" option. The same goes for copying directories!
Assuming you have a directory named "somedirectory", The syntax of copying a directory will look like this:
{% codeblock lang:bash %}
cp -rf somedirectory anotherdirectory
{% endcodeblock %}
Where "somedirectory" is the directory you want to copy and "anotherdirectory" is the name of the newly created directory that you want "somedirectory" to be copied into.
And that's all there is to that.  

Be sure that the last 3 posts make complete sense to you. If they don't please leave a comment or read them over again. In the next post I'm going to prepare you for programming in Ruby by setting up some "pre-ruby" stuff. See you in a few!
