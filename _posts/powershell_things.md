
# Powershell commands
> NOTE: Please read the official website if you're intrested in learning more in depth.<br>
> https://learn.microsoft.com/en-us/powershell/scripting/learn/ps101/00-introduction?view=powershell-7.5

### Intro
Hello, i am kulwanth(alias ikki) a computer science enthusiast and student i been using powershell all the time for last 3-4 months.
It made more productive with my work here are some very few commands that i use:

### 1. cd
  starting simple, cd means change directory, this command is used for moving from one directory
  
    cd ./Folder
  This result in moving to __Folder__ directory

    cd ..
  This result in moving from __Current directory__ to it's __Parent directory__

    cd ~
  This result in moving from __Current directory__ to __Home directory__

### 2. New-Item
  This is the LINUX's " touch " for powershell

    New-Item -Itemtype file -Path "./Folder/just.txt"
    ni -type f -Path "./Folder/just.txt" # short version
  This result in creating a file like __just.txt__ in your __Folder__ directory \
  you might say __"ikki i don't have a Folder for my just.txt"__
  well don't wory, try:

    New-Item -Itemtype directory -Path "Folder"
    ni -type d -path "Folder" # short version
  This should help you with making new directories.
### 3. mkdir
  mkdir means __make directory__ this is UNIX-based and what we use traditionaly

    mkdir Folder


    
