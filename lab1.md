Lab Report 1

# cd
1. Using '''cd''' with no arguments directs back to the start of the terminal since there is no directory to reference to.
~~~
[user@sahara ~]$ cd
[user@sahara ~]$
~~~
2. Using '''cd''' with a path directory such as '''lecture1''' changes directories to that path.
~~~
[user@sahara ~]$ cd /home/lecture1
[user@sahara ~/lecture1]$
~~~
3. When trying to do '''cd''' to a file, I get an error since I tried to change the directory into a txt file and a txt file is not a directory
~~~
[user@sahara ~]$ cd Hello.java
bash: cd: Hello.java: No such file or directory
[user@sahara ~]$
~~~

# ls
1. Using '''ls''' with no arguments show me '''lecture1''' since it is the only directory in the start.
2. Using '''ls''' with to a directory to messages shows me '''en-us.txt, es-mx.txt, fr.txt, zh-cn.txt''' since all the files are in the messages directory.
~~~
[user@sahara ~]$ /home/lecture1/messages
en-us.txt es-mx.txt fr.txt zh-cn.txt
[user@sahara ~]
~~~
3. Using '''ls''' to a txt file just points to the file itself since it's only a single file.

# cat
1. Using '''cat''' with no arguments keeps asking for input since there was no directory.
2. Using '''cat''' with a path to directory verifies if the path is a valid directory.
~~~
[user@sahara ~/lecture1]$ cat /home/lecture1
cat: messages: Is a directory
[user@sahara ~/lecture1]$
~~~
3. Using '''cat''' with a path to a file prints the contents in in the file.
