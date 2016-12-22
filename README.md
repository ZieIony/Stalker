# Stalker

### Team Member
##### GET /s/teamMember?app

Gets a list of team members for an app

##### POST /s/teamMember

Adds or changes a team member. Can be: Owner, Administrator, Developer, Tester, Client

 - only the app's owner can change the ownership
 - only administrators and the owner can add, change and delete team members
 - only the role can be changed in an existing team member
 - giving the ownership to a user makes the owner an administrator
 - fires a notification for affected users
 
##### DELETE /s/teamMember

Removes a team member

 - only the app's owner can remove an administrator
 - only administrators can remove other team members
 - the owner cannot be removed
 - fires a notification for affected user
