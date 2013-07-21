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
As you can see the name of the command was "touch" an it has 1 argument specifying the name of the file. In these cases the name of file would be "foo" or "bar".  
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
