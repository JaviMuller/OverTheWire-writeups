[comment]: # (Javier de Muller - 2023)

# Level 7

To enter the fourth level, you need to ssh into the same server and port with the user bandit7 and the password obtained
in the [previous room](lvl6.md).

From the goal, we can see that the password is next to the word 'millionth' in the file **data.txt**.
To find it, we use:

    $ cat data.txt | grep 'millionth'

which prints:

    TESKZC0XvTetK0S9xNwm25STk5iWrBvP
