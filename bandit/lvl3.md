[comment]: # (Javier de Muller - 2023)

# Level 3

To enter the third level, you need to ssh into the same server and port with the user bandit3 and the password obtained
in the [previous room](lvl2.md).

From the goal, we can see that the password is in a hidden file inside the **inhere** directory.
To read it, we use:

    $ ls -a inhere
    . .. .hidden
    $ cat inhere/.hidden

which prints:

    2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

