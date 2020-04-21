---
#### Identification

# Display name
name : {{ replace .Name "-" " " | title }}

# Nicknames (Names you use at articles or online. This allows you to be linked at articles.)
nicknames :
- {{ replace .Name "-" " " | title }}

# List the teams you're part of on this site.
teams :
- Badgeteam


#### Mini profile (Displayed at end of posts, where available)

# Avatar shown
avatar : "images/avatar.png"

# Short bio
bio : ""



#### Additional information for your personal page

# Full name (Shown on personal page only)
fullname : {{ replace .Name "-" " " | title }}

# Name icon (Shown in front of your name on profile)
icon_name : fa-address-card
icon_pack : fa

# Role/position (e.g., Professor of Artificial Intelligence)
role :

# Bodging area (The Hague, NL)
location :

# E-mail address to forward mail to. (Address not revealed at site)
email : ""

# Organizations/Affiliations
organizations :
- name :
  role :
  url  : ""

# List your interests
interests :
- Interest 1
- Interest 2

education :
  courses :
  - course      : Advanced badging and bodging
    institution : Bodgenatoric Institute
    year        : 2019

# Contact (Listed under personal details)
# For available icons, see: https://fontawesome.com
contact :
- title     : Webpage
  link      : https://www.my.site
  icon_pack : fa
  icon_name : fa-globe
- title     : Telegram
  link      : https://t.me/USERNAME
  icon_pack : fa
  icon_name : fa-telegram
- title     : Skype
  link      : https://skype.com/USERNAME
  icon_pack : fa
  icon_name : fa-skype

# Social (Listed in social-link bars)
# For available icons, see: https://fontawesome.com
social :
- title     : LinkedIn
  icon_name : fa-linkedin
  icon_pack : fa
  link      : https://linkedin.com/in/USERNAME
- title     : Twitter
  icon_name : fa-twitter
  icon_pack : fa
  link      : https://twitter.com/USERNAME
- title     : Reddit
  icon_name : fa-reddit-alien
  icon_pack : fa
  link      : https://reddit.com/user/USERNAME
- title     : Github
  icon_name : fa-github
  icon_pack : fa
  link      : https://github.com/USERNAME
---
