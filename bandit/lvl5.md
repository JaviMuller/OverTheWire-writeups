[comment]: # (Javier de Muller - 2023)

# Level 5

To enter the fourth level, you need to ssh into the same server and port with the user bandit5 and the password obtained
in the [previous room](lvl4.md).

From the goal, we can see that the password has 1033 bytes in size, is not executable, is human readable and should be inside the **inhere** directory.
To find it, we use:

    $ find inhere -size 1033c ! -executable -exec file {} \;
    inhere/maybehere07/.file2: ASCII text, with very long lines (1000)
    $ cat inhere/maybehere07/.file2

which prints:

    P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

