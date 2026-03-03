1. Setup moderator permissions  
By default, Gate can only be configured by people who have the administrator permission on discord. In order to allow non-admins to modify Gate's config, you'll need to grant one of their roles Gate moderation powers. You can do this in two ways:
- /server-config add-moderator-role: Adds one role to the list of Gate moderator roles.
- /server-config set-moderator-roles: Sets the list of Gate moderator roles to the ones you provide. This will overrride your pre-existing moderation role list, if you already had one.

2. Set up Discord permissions  
Next, make a discord role for every trust level you want to have. These roles will be mutally exclusive with one another, as a user's old trust role is removed as they gain trust levels. Configure your permissions with that in mind. Also, keep in mind that anyone who has not sent a message or interacted in your server since you added Gate will not have any of these roles.

3. Add trust levels to Gate, and configure cooldown  
Each trust level has three elements, Name, Role, and Threshold.  
Name: The name of the trust level.   
Role: The discord role members at this trust level will have.  
Threshold: The number of points needed to be at this trust level.  
You can add levels through /level-config add-level command, and remove them with /level-config remove-level  
Finally: You will need to choose the cooldown between gaining activity points. The default cooldown is 5 minutes, however this can be changed with /server-config set-activity-cooldown.   

Tip:  
It may be wise to not instantly lock channels if you are adding Gate to a well established server. Give users some time to gain points before everything is locked down.  
