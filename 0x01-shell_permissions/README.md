shell permissions
script that switches the current user to betty, betty will exist.

script that prints the current username
# whoami

script that prints all the groups the current user is part of.
# groups

script that changes the owner of the file hello to the user betty
#sudo chown betty hello

script that adds execute permission to the owner of the file hello.
#chmod u+x hello

script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.
#chmod 754 hello

script that adds execution permission to the owner, the groupowner and other users, to the file hello.
#chmod ugo+x hello

script that sets owner to no permissions at all, group no permissions at all and the users have all the permissions.
#chmod 007 hello

//

script that sets the mode of the file hello the same as olleh mode.
#chmod --reference=olleh hello

script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files are not changed.
#chmod -R +X .

script that creates a directory called my_dir with permissions 751 in the working directory.
#mkdir -m 751 my_dir

script that changes the owner to school for the file hello
# chgrp school hello

script that changes the owner to danteh and the group owner to staff for all the files and directories in the working directory.
#chown -hR danteh:staff .

script that changes the owner and group owner of _hello to danteh and staff respectively. _hello is a symbolic link.
#chown -h vincent:staff _hello

script that changes the owner of the file hello to betty only if its owned by the user guillaume.
#chown --from=guillaume betty hello