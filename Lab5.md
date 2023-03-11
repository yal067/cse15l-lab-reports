# Lab Report 5

# The process of doing lab report 3 and an alternative way doing it

## Going into detail on how to do the task of lab report 3

1.First, asking ChatGPT about some more commands and fuctions for "grep". For example, typing "what are some interesting commands for grep within a directory" in ChatGPT, it will provide many examples: ```grep -nr```, ```grep -c```,```egrep -i```, and so on.

2.After finding all the examples that seem useful or interesting, then try those commanda on files and directories from *./written_2*. For example: typing the command: ```grep -nr "Lucayans"``` in the terminal, the output will print the file's name that contains "Lucayans" which is *Bahamas-History.txt*, exhibits the line number that contains "Lucayans" in *Bahamas-History.txt* which is line 6 and line 7, and displays the content in those two specific lines.

3.Then, copying and pasting those to the file, and explaining the fuction of each specific command and the reason to pick this one as an example.

4.Importantly, don't forget to mention the references or resources where you find those useful commands.

## The alternative way of doing this lab report 3 - find

I will use the [website]([https://code.visualstudio.com/](https://linuxconfig.org/find)) to find some useful examples about the command ```find```

**find . -type f -name "files" -delete** 

This command will deletes files that is put in if we add the -delete option at the end. However, it will not display anything in the terminal after running this command.

**find /home -type d -name "directory"**

This command will only searches and displays directory that we want to find if we add -type d in the middle of this command. 

**find /home -type f -name "files"**

This command will only searches and displays files that we want to find if we add -type f in the middle of this command. 
