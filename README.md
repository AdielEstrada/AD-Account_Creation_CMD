# Part 3 - Using Active Directory and Using Common CMD commands, etc.

> [!NOTE]
> Have Server 2016 open with your administrator account. Open Active Directory Users and Computers (You can find it in the start menu under administrative tools, or you can search for it in the search bar). It would be useful if you kept this pinned to the taskbar, since we will be using this a lot.

## Finding Users in Active Directory
With Active Directory Users and Computers open, right click on any folder and click "Find".

<img src="https://i.ibb.co/PckhZKf/1-Find-in-active-directory-users-and-computers.png">

A pop-up will prompt you to name a user or an object. However, on the top, the folder you selected will appear. If you knew for certain a specific user was there, then you could leave as is. But, it's better if you switch out the folder for the entire directory just in case you missed the location of the user. So click on the folder (in my case the folder is called computers), and switch it for "Entire Directory".

<img src="https://i.ibb.co/rcK877H/2a-searching-goes-wrong.png">

This will enable you to search for users in a more accurate and efficient way. Now we can search users better. So, to try out this feature, search for any user. In this case, under "Name", we can search for "guest" by typing it in the search box. Click on "Find Now". Under "Search Results", you should find the listings that match your search.

<img src="https://i.ibb.co/2tTZ84y/3-searching-done-right.png">

## Using Advanced Features to Enable a More Detailed User Search
In Active Directory Users and Computers, you can go to the "View" tab. Click on Advanced Features. This will make more folders appear and enable a more advanced search. 

<img src="https://i.ibb.co/2qN51pf/4a-view-advanced-features.png">
