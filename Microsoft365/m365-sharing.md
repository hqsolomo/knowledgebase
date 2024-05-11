# Microsoft 365 Multi-Account Resource Sharing

Notes:  

* Unless otherwise noted administrator access will need to perform these steps  
* Any external users (accounts not controlled by the Microsoft account the shared resource is on) must be added as a guest user before performing these steps  

## 1. Adding Guest Users

1. Login to https://admin.microsoft.com  
2. Click `Users` then select `Guest users`  
3. Click `Add a guest user`  
  * If you are asked to select a user after clicking `Add guest user`  select the account you used to login with from step 1  
4. Click `Invite user` and enter the email address of the guest user  
5. Click `Invite`  
6. Confirm the user was able to accept the invite from their inbox  

## 2. Creating Microsoft 365 Groups

1. Login to https://admin.microsoft.com  
2. Click `Teams and groups` then select `Active teams & groups`  
3. Click `Add a Microsoft 365 group`  
4. Enter a name for the group then click `Next`  
5. Click `Assign owners` and select one or more owners for the group then click `Add`  
7. Click `Next`  
8. Click `Add members` and add one or more members, then click `Add`  
9. Enter a group email address and set the Privacy level  
  * It is recommended to set `Privacy` to `Private` unless you want users to freely access this mailbox without being approved by the owner first. For single-user organizations Public is a safe default  
10. Click `Next`  
11. Click `Create group`  

## 3. Adding Shared Folder/Mailbox to Outlook Web

* These steps should be performed by members of a Microsoft 365 group. This assumes you've accepted the invite email from section 1 above  

1. Login to your Outlook Web client  
2. Click the elipsis ("...") next to `Folders`  
  * You may have to hover your mouse pointer over the `Folder` label for the elipsis to appear  
3. Click `Add shared folder or mailbox` and enter the name or email of either the user that shared the resource with you  
  * If everything was set up correctly you should see `Suggested contacts` pop up when you click into the text box  
4. The shared folder/mailbox should be available at the bottom of the left panel  
  * You may need to refresh your page for the new item to appear  

## 4. Sharing Calendar

Prerequisites:  

* You have appropriate permission to share resources in your Microsoft 365 account  
* Your account administrator or Exchange administrator has not restricted sharing to the email address(es) you wish to share with  

1. Login to Outlook on the Web  
2. Click the `Settings` gear on the top left of the page  
3. Click `Calendar`  
4. Click `Shared calendars`  
5. Select the calendar you want to share in the `Share a calendar` dropdown, then click `Share`  
6. Enter the email address you want to share the calendar with  
7. Select the permissions you want that email address  
  * `Can view when I'm busy` shows reserved times on the calendars but _not_ what those reservations are for  
  * `Can view titles and locations` is similar to the above, but shows what the reservations are for  
  * `Can view all details` grants full read access to the calendar, but no edit access  
  * `Can edit` grants full read access to the calendar AND allows editing  
8. Confirm the recipient can access the shared calendar and can view/edit  
  * Recipient should be able to accept the invitation via email without error  
  * Tested with `outlook.office.com` (business email) and `office.live.com` (personal email). Also tested with `mail.proton.me`, though the calendar displays improperly in proton.  
