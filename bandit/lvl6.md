[comment]: # (Javier de Muller - 2023)

# Level 6

To enter the fourth level, you need to ssh into the same server and port with the user bandit6 and the password obtained
in the [previous room](lvl5.md).

From the goal, we can see that the password has 33 bytes of size and is owned by the user bandit7 and by the group bandit6.
In order to remove 'Permission denied' lines, we just pipe stderr to /dev/null.
To find it, we use:

    $ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
    /var/lib/dpkg/info/bandit7.password
    $ cat /var/lib/dpkg/info/bandit7.password

which prints:

    z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

