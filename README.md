# I passi della regina

By Davide Bucci

This project is the italian version of the text adventure game The Queen's Footsteps. It is written in the AWS language and it requires the AWS2C tool.

More information here:

https://github.com/DarwinNE/The-Queen-s-Footsteps

https://github.com/DarwinNE/aws2c

This game is distributed on Itch.io:

https://darwinne.itch.io/i-passi-della-regina

## Build and play

There is a build subdirectory for each computer system that is currently targeted by the game. The build is done using the make command on a Unix system.

This project should be a submodule of the AWS project, even if it can be used alone. When it is used as a submodule, once AWS is built it will refer to the AWS executable in the build directories (one for each computer systems) as ../../aws. If it is placed elsewhere, you will have to update the makefiles in the build directories.

The packaging of the executable is done by a script called produce.sh inside each build directory. There is a single common configuration file called config.sh that tells to the produce scripts where to find the packaging/disk access tools used to prepare the disk images, etc. for each computer. You will have to update it to refer to the commands of the tools installed in your system. 

## License

This project is licensed under the GPL v3 license.