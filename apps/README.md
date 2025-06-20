# Awesome Homelab


## Navigation
* [__Apps__](https://github.com/TechHutTV/homelab/tree/main/apps) - List of all the apps and services.
* [Home Assistant](https://github.com/TechHutTV/homelab/tree/main/homeassistant) - Smart home services and automation.
* [Media Server](https://github.com/TechHutTV/homelab/tree/main/media) - Plex, Jellyfin, *arr stack, and more.
* [Server Monitoring](https://github.com/TechHutTV/homelab/tree/main/monitoring) - Graphs and Visualizations for Unraid, Proxmox, and more.
* [Surveillance System](https://github.com/TechHutTV/homelab/tree/main/surveillance) - Frigate NVR Solution with Coral TPU.
* [Storage](https://github.com/TechHutTV/homelab/tree/main/storage) - Current Storage and Backup Solution.
* [Proxy Management](https://github.com/TechHutTV/homelab/tree/main/proxy) - NGINX Proxy Manager, DDNS with Cloudflare, Local Domains, and more.


In my network I also have two Raspberry Pis. One of them is a Pi 5 with a PoE HAT and that is responsible for a Twingate connector and updating my IP address on Cloudflare. The other is hooked up to a 3D printer running Octoprint.

## Dashboards

Dashboards are used to create a simple webpage with links to all the services, websites, or really anything you care about. What makes each dashboard special and unique is the features they come with. Many can act as monitoring tools, have widgets to get more details from services, weather, and more.

### Glance

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/01_glance-dashboard.png)

This dashboard is a new addition for me, it’s not the most feature rich of the options out there, but for me it’s simplistic and default look and feel is what stands out to me. You can use it to monitor and link to all your applications, like most tools in this category, but it also is great for monitoring various feeds, websites, and a customizable RSS feed. I use the tool as a start page for my web browser and it gives a quick and simple _glance_ of everything that I care about. One of the best things about it, in my opinion, is that everything is customized and configured in a simple yaml file.


### Portainer

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/05_portainer-docker-manager.png)

I’ll admit, I do have plans to slowly remove Portainer from my home server. I’ve gotten comfortable enough with using docker compose and other Docker features in the command line that it almost slows me down. With that said Portainer is a GREAT tool for managing Docker stacks, containers, and other instances on other machines.


## Media Server

### Jellyfin

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/08_jellyfin-media-server.png)

Jellyfin is by far the best free and open source media server on the market right now. It has all the features you’d expect without any paywalls. This includes streaming to a wide variety of platforms. I currently run Jellyfin as a backup to Plex as that is currently my preferred platform. See the video above for much more information.


### Plex

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/09_plex-media-server.png)

Plex is my main media streaming platform. I have quite a few family members using it and Plex has support for more platforms and easier login capabilities. I’ve also recently setup a TV tuner and it has been working great. Another reason why I use Plex is the support for 3rd party tools such as Tautulli that we will get into below.


### Tautulli

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/10_tautulli-plex-stats.png)

While Plex does have some statistics and logs to see what’s going on, it is nothing compared to what we get from Tautulli. From their website; “Tautulli is a 3rd party application that you can run alongside your Plex Media Server to monitor activity and track various statistics. Most importantly, these statistics include what has been watched, who watched it, when and where they watched it, and how it was watched.” This data is very helpful when I clean up and remove some media from the server. One of my favorite features of all this is the newsletter option that you can setup giving the users an overview of new media that has been added to the server.




## Filer Og Bilder

### Nextcloud

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/18_nextcloud-cloud.png)

Nextcloud is the best in the game for replacing cloud services like Google Drive, Onedrive, and so on. Not only can it act as a great on-premise cloud, but there are many other add-ons and features that it offers. This includes a complete groupware suite, collaborative document editing, tasks, and much more.

**Resources:** [Github](https://github.com/nextcloud) | [Website](https://nextcloud.com/)

### Immich

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/19_immich-photo-backup.png)

This is arguably the most important application that I am running. This is what I’ve used to completely replace Google Photos. Myself and a few of my family members use this as their primary Photo backup solution. It has a mobile app that supports easy backups and some other key features include facial recognition and a location map of your photos. From their website; “Easily back up, organize, and manage your photos on your own server. Immich helps you browse, search and organize your photos and videos with ease, without sacrificing your privacy.”

**Resources:** [Github](https://github.com/immich-app/immich) | [Website](https://immich.app/)

### Docmost

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/20_docmost-personal-wiki.png)

This is a new addition and it’s actually how I’m initially drafting this entire article. In my hunt to replace Notion I’ve started using this. While I’m still on a hunt for a more one-to-one replacement this is doing the trick for now. This tool is used to manage your own personal wiki, knowledge base, and notes. The UI is clean, elegant, and simple.

**Resources:** [Github](https://github.com/docmost/docmost) | [Website](https://docmost.com/)

## Smart Home and Automation

### Home Assistant

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/21_home-assistant-smart.png)

Home Assistant is a great tool that allows the connection of many devices in your smart home and integrate them together with a variety blueprints, automatons, and more. You can create custom dashboards, use their mobile app, and so much more I can’t even properly describe here how much this tool is capable of.

https://www.home-assistant.io/
**Resources:** [Video](https://www.youtube.com/watch?v=Y8xY4keybnw) | [Github](https://github.com/plexinc) | [Website](https://www.plex.tv/)

### Frigate

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/22_frigate-nvr.png)

Frigate is the best open source, self-hosted NVR option that I can find. For a while I was using Blue Iris, but I HATE that you have to use Windows. This tool shines with you hook it up with a Coral TPU for AI object detection. The interface is wonderful and it supports most of what you’d expect of an NVR. Granted depending on your cameras it may be difficult to configure and use all the features a camera may support, for example, two way audio.

**Resources:** [Video](https://youtu.be/NzbghOfRx3k?si=HY7aHdCbqz1X5ONe) | [Github](https://github.com/blakeblackshear/frigate) | [Website](https://frigate.video/)

### Zigbee2MQTT

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/23_zigbee2mqtt-smart-devices.png)

I was originally using this with Home Assistant as an add-on, but I’ve noticed it to be way more reliable if it is separated out. Zigbee2MQTT supports various Zigbee adapters and a bunch of devices.

**Resources:** [Github](https://github.com/Koenkk/zigbee2mqtt) | [Website](https://www.zigbee2mqtt.io/)

## DNS and Remote Connections

### Pi-Hole

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/24_pi-hole-dns-sinkhole.png)

By far the most popular “DNS Sinkhole” a Domain Name Service that blocks certain DNS inquiries. In the case of Pi-Hole it uses black lists full of domains associated with advertisements and tracking. For example, one of the most blocked domain on my server is [s2s.mparticle.com](https://www.mparticle.com/about-us/) a data collection firm. And with Pi-Hole I can investigate and figure out why this data collection company is being reached out to so much. This is in addition to the main use case of simple ad blocking. Pi-Hole has many other features I’ve yet to dive into, but it’s a wonderful tool that is worth trying out of anyone.

**Resources:** [Video](https://www.youtube.com/watch?v=xtMFcVx3cHU) | [Github](https://github.com/pi-hole/pi-hole) | [Website](https://pi-hole.net/)

### NGINX Proxy Manager

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/25_nginx-proxy-manager.png)

NGINX Proxy Manager is a simple web based proxy manager for setting up and forwarding domain names to your services and generating SSL certifications. I use this for both local top level domains and exposing a few select services to the public internet.

**Resources:** [Video](https://youtu.be/79e6KBYcVmQ?si=1h1daKy-0fZeiBtI) | [Github](https://github.com/NginxProxyManager/nginx-proxy-manager) | [Website](https://nginxproxymanager.com/)

### Twingate

Full disclosure, Twingate is one of the channel sponsors. This is a VPN alternative for remotely connecting to your home server. It works by spinning up a smaller connector on your local network, then you use a client to establish a secure peer-to-peer connection. All this is managed and verified through the Twingate cloud platform. Something I started using recently is the Twingate service API to connect with a headless client. Connecting to one headless service to another.

**Resources:** [Video](https://www.youtube.com/watch?v=yaw2A3DG664) | [Website](https://www.twingate.com/onboarding?utm_source=youtube&utm_medium=referral&utm_campaign=techhut-q1-25 )

### Cloudflare DDNS

![](https://github.com/TechHutTV/homelab/blob/main/apps/images/26_cloudflare-ddns.png)

This is a very simple docker container used to update your public IP address within the Cloudflare A records using their API. I need to use this because my public IP is dynamic, meaning it will randomly and automatically change every few weeks or sometimes every few days. From their Github it’s; “A feature-rich and robust Cloudflare DDNS updater with a small footprint. The program will detect your machine’s public IP addresses and update DNS records using the Cloudflare API.”





