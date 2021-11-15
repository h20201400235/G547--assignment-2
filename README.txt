Block Device driver (Disk on file)

| Download the main.c and Makefile

| Go to the directory in which code is downloaded and give the command $ make all

| Insert the module using sudo insmod main.ko

| use lsmod command to check if the module is loaded or not

| Check the partition info using cat /proc/partitions also check using ls -l /dev/dof* or sudo fdisk -l

|  2 logical Parititions of the Device(/dev/dof1 & /dev/dof2) are created

| Take root access using sudo -s command

|  use cat > /dev/dof to write into the disk. After giving the command, type something & press enter to read back from the disk on command line use command xxd /dev/dof | less

| Remove the module using sudo rmmod main.ko