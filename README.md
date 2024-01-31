## Mini Twitter

# A Java-based Mini Twitter with graphical user interface (GUI) using Java Swing. 

This is a pure desktop program, without web or mobile components. The goal of this assignment is to let me experience how to apply design
patterns to build extensible software systems.

The basic functions of the system include:
1. There is a centralized admin control panel to create users and user groups.
2. A user has 1) an unique ID; 2) a list of user IDs that are following this user (followers); 3)
a list of user IDs being followed by this user (followings); 4) a news feed list containing a
list of Twitter messages.
3. A user group has an unique ID, which can be used to group users. A user group can
contain any number of users. The same user can only be included in one group. Of
course, a user group can contain other user groups recursively. There is always a root
group called Root to include everything.
4. Users can choose to follow other users (not user groups) by providing the target user ID.
Unfollow is not required.
5. Users can also post a short Tweet message (a String), so that all the followers can see
this message in their news feed lists. Of course, the user can also see his or her own
posted messages.
6. A few analysis features are needed in the admin control panel: 1) output the total
number of users; 2) output the total number of groups; 3) output the total number of
Tweet messages in all the users’ news feed; 4) output the percentage of the positive
Tweet messages in all the users’ news feed (the message containing positive words,
such as good, great, excellent, etc.) Free free to decide the positive words.

I then built a GUI for the functions above:
1. All the UIs and layouts are just the suggested design for you to use. You can re-design
any of these as long as the functions are supported.
2. The Admin Control Panel is the main UI you will see by running the program. This should
be the entrance to the program.
3. You can add users/groups with Buttons and TextAreas. Of course, the TreeView should
be updated as well whenever new users/groups are being added.
4. For groups, you should display them with a different notation (maybe a folder icon or
something else just to distinguish it from the users).
5. Deleting users/groups is not required.
6. Clicking on the 4 buttons at the bottom-right will output the correspondent information.
You can simply popup a dialog to display the value, or use some other widgets.
7. When you select a user in the tree, clicking on the Open User View button will open the
User View as shown in Figure 2. You can open multiple User Views for different users.
8. In the User View, it will display the current users you are following in a ListView
(followings). You can add new users to follow by using the TextArea and Button.
Unfollow is not required. Displaying your followers is not required.
9. The User View also shows the current news feed list for this user in a ListView.
10. You can post a new Tweet with the TextArea and Button. Once you click the Post button.
It will add the message to all your followers’ news feed list, as well as your own news
feed list.
11. Whenever a new message is posted, all the followers’ news feed list view should be
updated and refreshed automatically.


You are encouraged to use as many design patterns as you can (even using the one we have
not covered in the class). The required patterns are Singleton, Observer, Visitor, and
Composite.
Your program should contain a Driver class with a main() method to trigger the Admin Control
Panel.
