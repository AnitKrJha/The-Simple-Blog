---
title: "Linux : Tips And Tricks 🎯📲"
date: 2022-08-18T16:20:46+05:30
draft: false
cover:
  image: "https://upload.wikimedia.org/wikipedia/commons/thumb/b/b0/NewTux.svg/640px-NewTux.svg.png"
  alt: "Linux Penguin Logo "
  caption: "Linux : Is the OS of serverse"

tags: ["Linux", "hugo"]
categories: ["Static Sites", "Tips&Tricks"]
---

# 10 Amazing Tips & Tricks to Work with Linux

Linux terminal can seem quite overwhelming for new users and even for experienced users without the knowledge of Linux tips & tricks. Linux is an incredibly flexible operating system.\
However, it is difficult to remember all the commands and their appropriate usage. Our amazing tricks will allow you to use Linux like a pro!

Take a look at these 10 tips & tricks to scale-up your Linux game:

## 1\. Removing Larger Files

Because of poor administrative skills files can get "heavy", sometimes as large as 250 GB! In that case, rm utility is not of much use due to the massive amount of data involved.

Therefore, removing a single log file of that size using rm utility should be avoided. You should rather opt for an easier solution:

```
 > /path-to-file/huge_file.log
```

You would be required to change file names and the path that matches your case. As a result, the empty output will be generated for that particular file.

## 2\. Copying in Multiple Directories

In general, when you want to copy a file, you use cp command which looks like this:

```
cp /path-to-file/my_file.txt /path-to-new-dir
```

Right? What if you want to copy that into multiple directories? You usually go for something like this:

```
cp /home/user/my_file.txt /home/user/1
```

Writing these commands over and over again is not only time consuming but frustrating as well. What if we tell you that you can still execute this process in a single-line command? Don't believe us? Try this:

```
echo /home/user/1/ /home/user/2/ /home/user/3/ | xargs -n 1 cp -v /home/user/my_file.txt
```

Voila! Your job is done.

## 3\. Minimizing Keystrokes

The more you press keys on your keyboard, the longer it will take to get things done. If you are aware of certain time-saving commands, you can increase your work efficiency by manifolds.

In order to execute your last command, you should make use of the UNIX bash shell.

Instead of typing the whole command again, just use Ctrl+R and change a few lines if you want to. That will save you a lot of time and speed-up your work.

## 4\. Searching Files Made Easy

This may seem easier than you think. Following is an example of the command used for searching files:

```
find /home/user -type f
```

Once you run this command, it will locate all files in /home/user. This is a powerful command but you may want to refine your search and make it more directed.

For instance, let's suppose you want to include an option to search files greater than 10 MB. You can do this by:

```
find . -type f -size 10M
```

Be careful not to use the root directory, failing which can cause high I/O on the system.

## 5\. Turning Off Your System

Did you know you can use certain commands to turn off your system at a specific time? You may or may not be physically present to shut down your computer but you can choose when to. Configure the shutdown time using this command:

```
sudo shutdown 21:00
```

Your system will shut down exactly at 21:00! Instead of hours, you can also choose minutes.\
For example:

```
sudo shutdown +15
```

Your computer will automatically turn off after 15 minutes.

## 6\. Using the Right Command

With several command lines at your disposal, it's extremely difficult to recall them when needed. Not only do you need to have the right command in mind, but also execute it effectively.

What you are looking for is this:

#apropos

Just replace "description" with the actual command description that you are searching for.

Take a look at this example:

- dir (1) -- list directory contents
- ls (1) -- list directory contents

With this trick, you don't need to recall the required command at all. You just need to search for one!

## 7\. Executing Multiple Commands

Quite often you have to wait for the previous command to run successfully in order to run the next one. This again consumes a lot of your precious time.

There's an efficient way to do it. You can use a single command to execute multiple ones and your waiting time is over!

The command looks like this:

command_1; command_2; command_3

This separator is a lifesaver when it comes to finishing your job within a stipulated time.

## 8\. Multiple Commands: When First One Fails

In the previous section, we talked about how to use a single command for running several commands. But what should you do in case the first command does not run successfully? You want to run the subsequent command only if the previous one was successful.

For this use "||" separator like shown below:

command_1 || command_2

After this, command 2 will run only after the command 1 when you use the above single-line command.

## 9\. Creating Directory Trees

You generally use the mkdir command to create new directories in Linux.

The usual command for creating directories goes like this:

```
mkdir new_folder
```

How about creating 7 sub folders within the new folder? Repeating the above command 7 times is not an ideal solution. You can instead use this command:

```
mkdir -p new_folder/{folder_1, folder_2, folder_3, folder_4, folder_5, folder_6, folder_7}
```

With the help of the above command, you can easily create 7 subfolders without having to run mkdir multiple times.

## 10\. Moving to End or Starting of Line

You have typed a lengthy command but realize that you need to move to the beginning of it in order to make some changes.

What do you do? Strike that left arrow key several times until you reach the starting of command?\
There is a better way.

Apart from using End and Home keys, you can opt for Ctrl+E to reach the end and Ctrl+A to reach the beginning.

## Inference

Mastering these tips and tricks will make your transition to Linux hassle-free.

The aforementioned commands are quite easy for everyone to comprehend even if they are not Linux experts. That's the beauty of it!

These useful tricks can work wonders for your efficiency. Wish you all the best for your Linux journey!
