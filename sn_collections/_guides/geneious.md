---
title: Geneious Software Guide
description: Geneious Software Use Guide
excerpt: Geneious Software Use Guide
## author: VRSC

categories: [Analysis]
---



Ceres no longer has Geneious Server. The developer has discontinued that product.

Ceres does provide floating licenses for Geneious Prime which is the desktop client.  


Caveats:
* The floating license server will only work at USDA sites or via VPN due to firewall restrictions.
* The Geneious Prime license server should work through both the regular USDA VPN and the SCINet ocvpn vpn servers. 
* If you do encounter license server issues let us know at [scinet_vrsc@usda.gov](mailto:scinet_vrsc@usda.gov)


First download the Geneious client from [https://www.geneious.com/download/](https://www.geneious.com/download/)

Install it as usual and start it up.

Geneious will complain about not having a license. Click "Activate a License"

![screenshot of Geneious software No License for Geneious R11 popup]({{ site.baseurl }}/assets/img/guides/analysis/geneious/geneious_license_expired.png)

On the "Enter Your License Details" screen,
  - select "Use floating license server",
  - enter `geneious.scinet.usda.gov` in the "License Server" box, and
  - enter `27001` in the "Port" box.

![screenshot of Geneious software Enter Your License Details screen]({{ site.baseurl }}/assets/img/guides/analysis/geneious/geneious_floating_license_server.png)


Geneious Prime can also be accessed via [OpenOnDemand]({{ site.baseurl }}/guides/software/open-ondemand)
which will allow you to run Geneious Prime directly on a cluster node.

![screenshot of Geneious in OOD menu]({{ site.baseurl }}/assets/img/guides/analysis/geneious/menu.png)
![screenshot of Geneious in OOD Options]({{ site.baseurl }}/assets/img/guides/analysis/geneious/options.png)
![screenshot of Geneious OOD launch]({{ site.baseurl }}/assets/img/guides/analysis/geneious/launch.png)
