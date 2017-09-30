# PA0 – Getting set up

This assignment is just for you to get set up with the accounts you need to do homework in this course. You won't be able to complete other work until it is done.

You will:

- Complete an academic honesty tutorial and submit a form
- Register your iClicker
- Register a Github account (and create one if needed)
- Log into the Raspberry Pi cluster
- Run a few commands to test out how we'll hand in work

Due Tuesday, October 3 by 11:59pm.

There are some frequently asked questions here:

https://piazza.com/class/j7w9htrxqm44j5?cid=23


## Academic Honesty/Plagiarism

Complete this tutorial:

http://libraries.ucsd.edu/assets/elearning/cse/cseplagiarismlink/story.html

Complete this form:

[Academic Honesty Agreement](https://docs.google.com/forms/d/e/1FAIpQLSfioSy3FLfg-xdPw_EYQe-_WQgpz0_hwk4jOGjtNwizmrlidQ/viewform)


## Log in to the Raspberry Pi cluster

Find your account by using the bottom form at:

https://sdacs.ucsd.edu/~icc/index.php

It should look like `cs30fXX` where `XX` are two letters. This is an account that is specific to you. You can use it to log into ieng6.ucsd.edu from anywhere via ssh, or onto the machines in the CSE labs.

The `ieng6` machines cannot run your assignments, though you can use them as usual for editing code, looking up online resources, etc.

From an `ieng6` machine (or from any computer on campus), you can log into the pi cluster using the same username and password, using the address `pi-cluster.ucsd.edu`. The command will look something like:

```
$ ssh cs30fXX@pi-cluster.ucsd.edu
```

If you're used to accessing the `ieng6` machines via PuTTY or another remote terminal tool, you can use that command from the terminal that's opened on `ieng6`.

The `ieng6` machines and the Rasperry Pis will all share your home directory, so anything you download or edit on one will be visible on the other – they are networked and using the same file system.

As part of this initial setup assignment we're going to copy a binary that will run on the Pis but not on the `ieng6` machines, to make sure the login has worked.

First, you will clone a repository we've made. Since the Raspberry Pis don't have external internet access, you will do this from the `ieng6` machine:

```
$ git clone https://github.com/ucsd-cse30-f17/pa0/
```

Then, from the Pi, run the following command:

```
$ ./pa0.bin
Hello, cs30f!
A number: <some number>
```

If you accidentally run it on the `ieng6` machine, you'll just see this output:

```
$ ./pa0.bin
-bash: ./a.out: cannot execute binary file
```

## iClicker Registration, Github account setup, and Handin

Complete this form so we can associate your various accounts, and paste the output of `./pa0.bin` above as the answer to the last question:

[Account Registration Form](https://docs.google.com/forms/d/e/1FAIpQLScuZfh_JQsksLSXHupoRJ9KClLMoxrHB8wPbjEAZCe9XKwm-g/viewform)
