[comment]: # (Javier de Muller - 2023)

# Level 4

To enter the fourth level, you need to ssh into the same server and port with the user bandit4 and the password obtained
in the [previous room](lvl3.md).

From the goal, we can see that the password is in the only human-readable file inside the **inhere** directory.
To find it, we use:

    $ find inhere/* -exec file {} \;
    inhere/-file00: data
    inhere/-file01: data
    inhere/-file02: data
    inhere/-file03: data
    inhere/-file04: data
    inhere/-file05: data
    inhere/-file06: data
    inhere/-file07: ASCII text
    inhere/-file08: data
    inhere/-file09: data
    $ cat inhere/-file07

which prints:

    lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

