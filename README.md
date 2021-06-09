
## Permissions



Linux permissions dictate 3 things you may do with a file, read, write and execute. They are referred to in Linux by a single letter each.



__r__ (read) - you may view the contents of the file.
__w__ (write) - you may change the contents of the file.
__x__ (execute) - you may execute or run the file if it is a program or script.



For every file we define 3 sets of people for whom we may specify permissions.



#### Owner



The user who owns the file. Typically the person who created the file but ownership can be changed.



#### Group



Every file belongs to a single group. Groups can have many users in it so you can give access to multiple people.



#### Others



Everyone else who is not in the group or the owner.




Three persmissions and three groups of people. That's about all there is to permissions really. Now let's see how we can view and change them.



### View Permissions



To view permissions for a file we use the long listing option for the command ls.



ls -l [path]



### Change Permissions



To change permissions on a file or directory we use a command called "chmod" It stands for change file mode bits which is a bit of a mouthfull but think of the mode bits as the permission indicators.



```
chmod [permissions] [path]
```



chmod has permission arguments that are made up of 3 components



There are two ways you can use chmod and you will see both used. One is shorter and one is more descriptive.
