---
layout: post
title: "how to use the Terminal (part 2)"
date: 2013-07-20 13:39
comments: true
categories: ["Terminal", "Commands", "Files", "Folders", "Directories"]
---

Welcome back Maddie! If you haven't read the [first part](http://dillon-benson.github.io/blog/2013/07/18/how-to-use-the-terminal/) of this tutorial, I strongly suggest that you do. If you have already read it, then you should be ready for this tutorial. In this post I will cover creation and deletion of files, how to delete directories the right way, and quickly find out what's inside of a file. All this will be done with the power of the terminal. Remember, I strongly advise you to read the [first section](http://dillon-benson.github.io/blog/2013/07/18/how-to-use-the-terminal/) before this.  

##Creating and deleting files
Creating and deleting files is an important part in becoming good with the terminal. Let's first start with creating files. Creating files is similar to creating a directory with the "mkdir" command from the previous section. However instead of using "mkdir" we use the "touch" command. The main purpose of "touch" is to generate a file with whatever name you want. To specify the name of the file you just pass the "touch" command an argument:
{% codeblock lang:bash %}
touch foo
{% endcodeblock %}
where "foo" would be the name of the newly created file.  
or
{% codeblock lang:bash %}
touch bar
{% endcodeblock %}
where "bar" would be the name of the newly created file.  
As you can see the name of the command was "touch" and it has 1 argument specifying the name of the file. In these cases the name of file would be "foo" or "bar".  
Deleting files is pretty straight foward. You do this with the "rm" command. "rm" is short for remove. Just like the "touch" command, "rm" takes 1 argument specifying the name of the file that you wish to delete. Let's say you have a file named "foo". When you use the "ls" command you should see something like this:  
{% img /images/ls-foo.png %}  
See the file named "foo". Now you want to delete it. To do that you would just use:
{% codeblock lang:bash %}
rm foo
{% endcodeblock %}
"foo" is the only argument to the "rm" command this time.  
Now when you use the "ls" command you see it has been deleted and disappeared from the directory.
{% img /images/ls-foo-deleted.png %}
Like this.  
Now that you got the hang of creating and deleting files, it's time to show you how to delete directories.  

##Deleting directories
Removing a directory is just like removing a file. In fact it's the same command, "rm". However, it's time to introduce a new concept to commandss. You know that commands have 0 or more arguments.
{% codeblock lang:bash %}
cd foo
{% endcodeblock %}
This has a command, "cd", and an argument, "foo". Turns out that commands have another nice features called options and they're a special form of arguments. Options are arguments that are prefixed with "-" or "--". The main purpose of options are to specify how you want a command to be run. Keep in mind however that not all commands have options. It turns out that the "rm" command has a special option for deleting directories. "-rf". This means remove a directory with recursive force. Don't worry about what that means for now. Just know that "-rf" along side of "rm" is used for deleting directories. Let's say our home directory looks something like this:
{% img /images/foo-directory.png %}
Notice the "foo" directory? If we want to delete this, all we need to do is issue an "rm" command like this:
{% codeblock lang:bash %}
rm -rf foo
{% endcodeblock %}
Where "rm" is the remove command, "-rf" the recursive force option we're using, and "foo" being the argument specifying the directory we want to remove.  

##showing what's in a file
There a nice command called "cat" that's used for showing what's inside of a file. Let's say that sometime in the future when you begin programming your first ruby code you have a file named "hello.rb" (The ".rb" in the file name means it's a ruby file). Now if you want to see what's inside of this just use "cat" with an argument. As you might have already guessed, yes, "cat" takes one argument specifying the name of the file you want to see the content of. So issuing:
{% codeblock lang:bash %}
cat hello.rb
{% endcodeblock %}  
May result in something that looks like this:  
{% img /images/cat-hello-rb.png %}
Below the "cat" command you see ruby code. This is what's inside of the "hello.rb" file. Ruby code!  

I hope this tutorial went good for you. If you have any questions please leave a comment. Make sure you have a good grip on what you've learned so far. We're not done with the terminal tutorials yet. It's crucial you understand how to use it before you begin programming. Thanks for reading. See you soon.
