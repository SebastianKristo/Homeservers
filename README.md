# My Homeserver Setup


## Navigation
* [Apps](https://github.com/TechHutTV/homelab/tree/main/apps) - List of all the apps and services.
* [Home Assistant](https://github.com/TechHutTV/homelab/tree/main/homeassistant) - Smart home services and automation.
* [Media Server](https://github.com/TechHutTV/homelab/tree/main/media) - Plex, Jellyfin, *arr stack, and more.
* [Server Monitoring](https://github.com/TechHutTV/homelab/tree/main/monitoring) - Graphs and Visualizations for Unraid, Proxmox, and more.
* [Surveillance System](https://github.com/TechHutTV/homelab/tree/main/surveillance) - Frigate NVR Solution with Coral TPU.
* [Storage](https://github.com/TechHutTV/homelab/tree/main/storage) - Current Storage and Backup Solution.
* [Proxy Managment](https://github.com/TechHutTV/homelab/tree/main/proxy) - NGINX Proxy Manager, DDNS with Cloudflare, Local Domains, and more.

## Hardware

![counter top lab](https://github.com/TechHutTV/homelab/blob/main/storage/homelab.png)

#### Aoostar Wrt Pro (Unraid)
This machine is running Proxmox. Due to a free PCIe slot this has an additional Coral TPU and I'm currently testing it with Blue Iris. Running Immich for personal photo backups and MeTube to pull YouTube videos for use in media projects. This machines handles the network shares that connect to our Nextcloud instance.
* 12th Gen Intel Core i5 1235U
* [16GB SODIMM DDR5](https://amzn.to/3YqeZ9A)
* [DataTraveler 3.0 32GB USB](https://amzn.to/4fovZUR) (Boot Drive)
* x1 [Seagate IronWolf 16TB NAS HDD](https://amzn.to/4eNPXYv) (Parity Drive)
* x5 [Seagate IronWolf 4TB NAS HDD](https://amzn.to/3Y6eyT7) (Raid5 Pool)
* x2 [T-Create 1TB 2280 NVMe](https://amzn.to/4dGvwMx) (Cache)

#### Intel NUC (Ubuntu)
This NUC has a base install of Ubuntu 24.04 with docker. This machine is dedicated to business services including Odoo and Nextcloud.
* 13th Gen Intel i7-1360P
* [32GB SODIMM DDR5](https://amzn.to/3Um77VB)
* [Intel 670p Series M.2 2280 512GB](https://amzn.to/40fOiHn) (Boot Drive)

### Networking
#### UniFi
* [TP-Link Omada Hardware Controller](https://amzn.to/48vW6H1)



