
# Powershell commands
> NOTE: Please read the official website if you're intrested in learning more in depth.<br>
> https://learn.microsoft.com/en-us/powershell/scripting/learn/ps101/00-introduction?view=powershell-7.5

### Intro
Hello, i am kulwanth(alias ikki) a computer science enthusiast and student i been using powershell all the time for many months.
It made more productive with my work here are some very few commands that i use:

### 1. cd
  starting simple, cd means change directory, this command is used for moving from one directory
  
    cd ./Folder
  This result in moving to __Folder__ directory

    cd ..
  This result in moving from __Current directory__ to it's __Parent directory__

    cd ~
  This result in moving from __Current directory__ to __Home directory__

    cd /
  This result in moving from __current directory__ to __Root directory__

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
  Also if you want to create a directory inside 1/many directories use:

    mkdir -p "BiG Folder/sub-BiG Folder/Folder"
  The __-p__ will create the BiG Folders if they don't exist.

### 4. rmdir
  rmdir means __remove directory__

    rmdir Folder

### 5. cat
  When you want to look-up what is inside a file, you use __cat__ to do it.

    cat file.txt

### 6. notepad
  In powershell, you can open text file (or new text file) with notepad

    notepad
    notepad file.txt
    
### 7. saps & spps
  saps => start's a process <br>
  spps => stop's a process

    $ps1 = saps powershell -PassThru
    spps -Id $ps1.Id -Force
  I'm not to sure! about how i can use them but it's cool (I Think?).

### 8. shutdown
  As you might have guessed it shutdowns

    shutdown /s /t 0

### 9. sleep
  This adds __delay__ between processes that you are running on your system.

    sleep -second 2
  This should keep the shell in 2 seconds of sleep.

### Something Fun:
  Today before you shutdown your System/Computer do this:

    clear;1..5 | % {
    Write-Host "..$_"; sleep -second 0.65;
    };Write-Host "`nByee..Byee..";sleep -second 0.65;shutdown /s /t 0;
  Just for fun __DO IT!__
  Also you can try repalcing __Write-Host "`nByee..Byee..";__ with

    clear;1..5 | % {
    Write-Host "..$_"; sleep -second 0.65;
    };Write-Host "`nByee..Byee.." -ForegroundColor Magenta;sleep -second 0.65;shutdown /s /t 0;
  OOH.. It looks better with some little color
