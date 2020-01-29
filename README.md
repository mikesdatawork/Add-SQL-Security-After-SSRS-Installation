![MIKES DATA WORK GIT REPO](https://raw.githubusercontent.com/mikesdatawork/images/master/git_mikes_data_work_banner_01.png "Mikes Data Work")        

# Add SQL Security After SSRS Installation
**Post Date: April 15, 2015**        


## Contents    
- [About Process](##About-Process)  
- [SQL Logic](#SQL-Logic)  
- [Build Info](#Build-Info)  
- [Author](#Author)  
- [License](#License)       

## About-Process

<p>Once you have SSRS 2012 installed, and configured, one of the most important things you should do is configure security for SSRS. By default all groups are essentially relegated as a basic user (regardless if you have been added as admin or not). UAC will always block access to users or applications trying to add/create/edit reports via SSRS. The solution is to simply configure security within reporting services to add the BuiltinAdministrators (or other group the admins are a part of locally on the server). Here is the process for that.
From the database server where you have installed SQL Server Reporting Services.
Open the browser with Administrative rights.</p>

![run as admin]( https://mikesdatawork.files.wordpress.com/2015/04/image001.jpg "Click Run As Admin")
 
Go to this address:
http://MyServerName/Reports_MyInstanceName
Click Site Settings link on the right.

![SSRS Site Settings]( https://mikesdatawork.files.wordpress.com/2015/04/image002.jpg "Click Site Settings")
 
Click the Security button on the left.

![Site Settings]( https://mikesdatawork.files.wordpress.com/2015/04/image003.jpg "Click Security")
 
Check the box next to BUILTINAdministrators, and click 'Edit'.

![Click Edit]( https://mikesdatawork.files.wordpress.com/2015/04/image004.jpg "Select Edit")
 
Select 'System User', and click 'Apply'.

![Select System User]( https://mikesdatawork.files.wordpress.com/2015/04/image005.jpg "Click Apply")
 
You're done.
Easy peasy.

[![WorksEveryTime](https://forthebadge.com/images/badges/60-percent-of-the-time-works-every-time.svg)](https://shitday.de/)

## Build-Info

| Build Quality | Build History |
|--|--|
|<table><tr><td>[![Build-Status](https://ci.appveyor.com/api/projects/status/pjxh5g91jpbh7t84?svg?style=flat-square)](#)</td></tr><tr><td>[![Coverage](https://coveralls.io/repos/github/tygerbytes/ResourceFitness/badge.svg?style=flat-square)](#)</td></tr><tr><td>[![Nuget](https://img.shields.io/nuget/v/TW.Resfit.Core.svg?style=flat-square)](#)</td></tr></table>|<table><tr><td>[![Build history](https://buildstats.info/appveyor/chart/tygerbytes/resourcefitness)](#)</td></tr></table>|

## Author

[![Gist](https://img.shields.io/badge/Gist-MikesDataWork-<COLOR>.svg)](https://gist.github.com/mikesdatawork)
[![Twitter](https://img.shields.io/badge/Twitter-MikesDataWork-<COLOR>.svg)](https://twitter.com/mikesdatawork)
[![Wordpress](https://img.shields.io/badge/Wordpress-MikesDataWork-<COLOR>.svg)](https://mikesdatawork.wordpress.com/)

    
## License
[![LicenseCCSA](https://img.shields.io/badge/License-CreativeCommonsSA-<COLOR>.svg)](https://creativecommons.org/share-your-work/licensing-types-examples/)

![Mikes Data Work](https://raw.githubusercontent.com/mikesdatawork/images/master/git_mikes_data_work_banner_02.png "Mikes Data Work")

