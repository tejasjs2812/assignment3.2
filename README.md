# assignment3.2

Que1)Create a file with the name max-temp.txt in the local file system and add
10-15 records with two columns for date and temperature and save it as
max-temp.txt
--commands--
touch max-temp.txt
vim max-temp.txt
i
put 10-15 records
esc
:wq

Que2)Copy the above max-temp.txt file from the local file system to HDFS in the
/user/acadgild/hadoop path.
--command--
hadoop fs -put max-temp.txt /user/acadgild/hadoop



Que.3)Change the permission of the file /user/acadgild/hadoop/max-temp.txt,
such that only the owner and the group members should have the r-w-x
permissions. Others should have only read the permission on the above file.
--command--

hadoop fs -chmod u=rwx,g=rwx,o=r /user/acadgild/hadoop/max-temp.txt
