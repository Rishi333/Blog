---
title:  "Harmony with Apache and Nginx"
header:
  teaser: "https://farm5.staticflickr.com/4076/4940499208_b79b77fb0a_z.jpg"
categories:
  - Jekyll
tags:
  - innovations
---

Port listening and forwarding is a living hell that I wouldn’t even wish it upon my worst enemy. However, if you are going to run both Apache and Nginx on a single server, then you have no choice but to become Dante and embark on your trek into the inferno. In my own specific use case, I wanted to set up gitlab and suitecrm. However, I already had my suitecrm set up with apache2 and did not want to take the extra hassle to convert to Nginx. Also gitlab uses Nginx through Chef and builds Nginx configuration at runtime. Thus, in order to save myself precious time, I made a simple change to the apache2 configuration. I defaulted the listening port on apache2 to port 8001. This fix allowed me to run Nginx as the primary server and Apache as a secondary server. Nginx is known to provide speed upgrades compared to apache2, thus it made more sense to setup the server in this fashion. 

<figure>
  <img src="/Blog/images/nva.png">
</figure>