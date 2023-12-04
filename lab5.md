## Part 1

Student: Hello, I'm doing the code for the handleRequest method for the Lab Report 2 writeup and when I'm running the StringServer I only get one line of output instead of multiple lines do you know how I can fix this? Here is my code and the output it's giving:

![Image](1lab.png)
![Image](3lab.png)
![Image](4lab.png)

TA: Think about how strings work and how it connects to reloading your page on the web server. When entering data in your query think about why your previous inputs are being overwritten.

Student: Alright I will try that. I see that for my message variable that I needed to do += instead of just = to my data that I am displaying.

![Image](2lab.png)
![Image](6lab.png)

[Information needed about the setup]

Here is the file directory & structure that I need which is just Server.java, run.sh, and StringServer.java

![Image](5lab.png)

Here are the contents of the StringServer.java before fixing the bug

![Image](7lab.png)

The command line I triggered the bug was `http://localhost:4000/add-message?s=Hello`, `http://localhost:4000/add-message?s=World`, and `http://localhost:4000/add-message?s=Song Birds` 

To fix the bug add += for my message variable

![Image](8lab.png)

## Part 2

In the second half of the quarter what I thought was really interesting thing to learn
was vim. Learning vim, I learned that I can edit my code just from my terminal and that an
IDE is not the only thing that I can use to edit code with.

learn bash, jdb, and vim to efficiently debug my code.
I learned how to use bash to report errors in my code and used bash to report how to fix my code.
I also learned to efficiently debug my java code using jdb such as using the "stop at" command to find a breakpoint in my code where the errors are showing. 
What I thought was really cool was that I learned that I don't even need an IDE or even Notepad to edit my files, 
I can just edit files from my terminal with git commands and using vim.
I learned git commands to save my changes with just the command lines with git add and git commit instead of going to the github to save my changes.
I also learned how to apply jdb, vim, and git in lab for my ChatServer lab project.
