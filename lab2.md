# Lab 2 - Command Line Practice

After an admittedly stressful lab 1 in Excel, I thought it would be good to give you a nice treat with Lab 2. 

This week, there is only one task for you: practicing the command-line through a game along with working with Git commands.
Watching Dr. Moosvi's video before completing the lab would be helpful.


[![](http://img.youtube.com/vi/QtxwgG2u6Uc/0.jpg)](https://www.youtube-nocookie.com/embed/QtxwgG2u6Uc "")



**This lab must be completed individually.**

## Objectives

- Practice with command-line interfaces
- Create and navigate directories
- Create, modify, rename and delete files
- Understand basic Git commands and Git fundamentals

## Marking and Evaluation (20 marks)

**Step 1: Accept the lab assignment**
You can find the link to accept the lab on Canvas.

**Step 2: Clone the repository on your local computer and navigate to that directory**

As with Lab 1, you will need to clone the GitHub repository somewhere locally.
The steps to do this are:

1. `cd /path/to/where/you/want/labs` or `go to your directory and open Git Bash there!`
2. `git clone https://github.com/data301-2020-winter1/lab2-yourUserName`


## Part 1,2: Practicing with Command Line (70% - 14 marks) , working with Git Commands (30% - 6 marks)

Here is a guide to the first few steps of the activity.

### Setting up for the game

1. Open a Terminal window.( gitBash)
2. Change the directory to where this file is: `cd /path/to/this/folder`.
3. Type `ls` into the Terminal; you will see two things: `README.md` and the `entrance` directory.
4. Once you go into the `entrance` directory (`cd entrance`), the command line based game will begin!

**Tip: When I say "go into the <BLANK>" room, I mean change directories using `cd <BLANK>`. In this game, a "room" is a "directory".**

### Starting the game

5. Now that you have entered the dungeon `entrance`, you should type `ls` in the terminal to look around and see what's there.
6. You will see there are two "things" in this room,  there is a `scroll`, and another room called `cellar`.
7. Let's read the scroll using `cat scroll`.

**Tip: When I say "read the scroll", I mean output the contents of the scroll file into the Terminal using `cat scroll`.**

8. Great! The scroll told us that we can look and see what's in the room using `ls` and move in and out of rooms using `cd <directory>`. 
    
9. To keep track of directories you've been so far, let's make a text file "breadcrumbs.txt" and add some info to it, to do so, you sould run these commands:   
    `echo "your name, been here!" > breadcrumps.txt`
    
10. Once you run this command you should add this new file to the github repository and make a commit, so while you're still in the same directory, run the following commands:
```
    `git add breadcrumps.txt`
    `git commit -m "a meaningful message to remember later"`
    `git push`
 ```
 
**Tip: afterwards, when I say "push to Git", I mean run the three commands above! By running these commands, you basically will have a snapshot of what you have been so far in this game!**
   
11. Let's go into the cellar: `cd cellar`.

12. Once we're in the `cellar`, let's have a look around: `ls`. You should see an `armoury`, a `scroll`, and some `treasure`.

13. Let's read the scroll: `cat scroll`. It should tell you about `ls -F`. Here is some more information about `ls -F`:

> Display a slash (`/') immediately after each pathname that is a directory, an asterisk ('*') after each that is executable, an AT sign ('@') after each symbolic link. 

14. That sounds useful, let's do an `ls -F` in the cellar to see what each of the things are. You'll notice that the armoury is another room, the scroll is just a file, and the treasure has a "*" at the end, so it's an executable. Cool! We don't know what to do with the executable yet, but let's try `cat treasure` to see what happens.

15. Mm. Didn't work - okay let's move on and come back to this room later. Let's go into the `armoury` now: `cd armoury` and then `ls -F`.

16. We see another scroll (and a potion, a treasure, and another room)! Let's read the scroll: `cat scroll`.

17. Oooh, we have now learned how to collect `treasure`! Let's do that in the armoury and follow the instructions to keep our treasure (using environment variables).

**Tip: When I say "pick up the <BLANK>", I mean run the executable file using `./ <BLANK>`.**

16. It tells us to go back and get the treasure from the cellar! but before going there, let's leave a breadcrumps here! make another text file in this repository as I explained in *9*.

17. It's time to push to Git again! Don't worry, see *10* if you forgot what to do!
    
18. Let's go back now with `cd ..`, and pick up the treasure from the cellar, and then come back to the armoury.

16. The potion is also something we can "pick up", so let's go ahead and do that. It asks us if you want to drink it: type 'Y' for yes, and anything else for no (like 'n'). Choose an option and see what happens (follow on-screen instructions!)

17. Alright check if there's anything else to do this in room, if not, head to the `chamber` next. Start with `ls -F` and hopefully by now, you know the drill!

18. Have fun! More dungeon rooms will open up as you complete certain tasks, kill certain monsters, and read specific scrolls and tomes. Have fun with it, this is your opportunity to practice your Terminal skills - it sure beats the way I learned Terminal commands (blindly typing in commands in a black box until I got it to do what I wanted!). There is no need to hit **every** room in the dungeon, but do make a concerted effort (you should at least have 3 'breadcrumps.txt' files  and 3 commits respectively in total) and you'll likely get most of the marks for this lab. 

**Tip: You can ignore a few of the more "advanced" entries of the Tome, including anything related to `tmux` or `gzip`. I say "pick up the <BLANK>", I mean run the executable file using `./ <BLANK>`.**

### What you need to submit for this assignment.

When you're done exploring the dungeon this is I want you to do:

#### 1. Commit everything to your repository and push to the cloud:

```
git add .
git commit -m "Finished playing with the dungeon"
git push
```



#### 2. Save the last 100 commands from your Terminal

We want to see some serious effort with the dungeon map, so we are asking for the last 100 commands you entered into the Terminal.
Please open this file and do a quick check to make sure there is no sensitive information in this file (like passwords or private messages).
If there is, you can simply edit file or remove that command.

**Note: Just because we're asking for the last 100 commands doesn't mean that we expect you to have 100 commands, you may have less and you may have more. That's fine.**

```
history 100 > dungeonHistory.md
```
#### 3. Commit the dungeon history to your repository 

Run the following commands in your Terminal:

```
git add .
git commit -m "Added my dungeon map"
git push
```

#### 4. Submit the link to your GitHub.com repo to Canvas

You're done! 


## Attribution

The `bashcrawl` game was adapted from `@slackermedia` on GitLab.
FULL Credit for the game goes to [Seth Kenlon](http://slackermedia.info/about/).
The link to the game source code is [here](https://gitlab.com/slackermedia/bashcrawl).
