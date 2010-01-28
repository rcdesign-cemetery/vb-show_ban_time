Description:
------------

vBulletin addon. Show ban expiration time after group name

- in profile
- in postbit
- in private messages

Don't forget to select "blocked" groups, that should have this feature on.

!!!

thread SQL code is not optimal. Query should be fixed first in showthread.php, line 1001:

IF(displaygroupid=0, user.usergroupid, displaygroupid) =>
IF(user.displaygroupid=0, user.usergroupid, user.displaygroupid)

http://www.vbulletin.com/forum/project.php?issueid=35757 


