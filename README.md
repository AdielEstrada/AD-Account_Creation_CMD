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

As you can see, more folders will pop-up. We can ignore this for now, but we will begin our search again. The process is the same. We are still searching for guest, so we will still search for the guest in the entire directory. But now, when we see the user named "Guest" in the search results, we will want to right click on that user. After that, we will want to look at the Properties option. 

<img src="https://i.ibb.co/7QpnBwP/7-guest-search-up-and-properties.png">

A pop-up called guest properties will appear. Here, in the General tab, we will find general information about the user. However, since we enabled advanced features, we get more tabs we can explore. For example, one of the tabs that gives useful information is the Object tab. So, click on Object. 

<img src="https://i.ibb.co/S58zsYw/8-properties-object.png">

The Object tab will pop-up. This tab helps us identify what groups a user is part of. So, this user is part of the "adielit.local" domain, and part of the "Users" group. Knowing what groups the guest or any user for that matter is part of, you can know what policies are implemented. 

<img src="https://i.ibb.co/YjgZ3PR/9-what-object-shows-1.png">

## Enabling the Recycle Bin in Active Directory Administrative Center

In the start menu, or in the search bar, look for "Active Directory Administrative Center" (If you are using the start menu, go to Windows Administrative Tools). Open the app. 

<img src="https://i.ibb.co/pZwtPKR/11-enablerecyclebin.png">

Then, there will be a pop-up asking us to confirm whether we want to enable the recycle bin. We can confirm by pressing ok.

<img src="https://i.ibb.co/bQG1HLb/12-ok.png">

Then, another screen will prompt us to refresh AD Admin Center. We can press ok, and press the refresh button up on top. 

<img src="https://i.ibb.co/6sN4kCY/13-refreshing.png">

A new folder should pop-up, named "Deleted Objects". This indicates that the recycle bin has been enabled correctly. 

<img src="https://i.ibb.co/CQ546gy/14-shows-up-as-deleted-objects.png">

## Creating Users in Active Directory
To create a new user, open Active Directory Users and Computers. Usually, you would right-click on an empty space, and click new, then user, and go on to create the account with suitable permissions. However, in this case, we want to replicate an administrator account so that we can do more experiments on the desktops we will be virtualizing. Therefore, the process to create this special account is as follows.

In Active Directory Users and Computers, open the "Users" folder. Right click on Administrator, and choose copy. 

<img src="https://i.ibb.co/dcg2X2X/15-right-click-on-admin-and-copy.png">

A screen prompting you to name the new user will pop-up. You can name the user whatever you want for this environment. In my case, I named my user "helpdesk", as it will help me to identify the account much easier. The logon name should be "helpdesk" as well. After that, we can click next. 

<img src="https://i.ibb.co/10GsbC0/16-creating-helpdesk-account.png">

Then, it will prompt you to create a password. Make sure the password is simple to remember in this case, since we will need quick access to the password. Once you've created the password, confirm it and make sure the only box that is checked is the one that says that the password never expires. 
