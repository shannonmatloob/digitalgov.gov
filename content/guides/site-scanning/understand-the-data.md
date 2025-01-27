---
date: 2020-07-28 09:00:00 -0500
title: "Understand the Data"
deck: ""
summary: ""
guide: site-scanning
aliases:
  - /guide/site-scanning/understand-the-data/
  - /guide/site-scanning/understanding-the-data/
---

The Site Scanning engine runs against the full list of federal goverment websites and analyzes various aspects of them.  

The scans operate without authentication over the public internet. Using a headless browser (a browser without a graphical interface), they load each Target URL and inspect what would normally be returned to a user who is visiting that page with a web browser.  The results of these inspections form the data that Site Scanning makes available.  A more detailed description of how the scans operate can be found [in the documentation repository](https://github.com/18F/site-scanning-documentation/blob/main/pages/how-the-scans-work.md).  

The scans currently collect the following data about each target URL.  A complete data dictionary with much more detail can be found [in the documentation repository](https://github.com/18F/site-scanning-documentation/blob/main/pages/data-dictionary.md).


| General  |  USWDS | DAP  | SEO  | Third Party Services  |
|---|---|---|---|---|
| Server Response Code  | Presence of USWDS components  | Presence of DAP snippet | Meta Description Tags  | Presence of Third Party Services  |
| Redirects  |  USWDS Version | Customizations of the Snippet  | Presence of Robots.txt  | Number of Third Party Services   |
| Domain  |  Degree of Implementation |   |  Elements of the Robots.txt |   |
|  Agency Bureau |   |   | Presence of Sitemap.xml  |   |
| Bureau  |   |   | Elements of Sitemap.xml  |   |
|  404 Configuration |   |   |   |   |

  
_Have ideas for what else we should be scanning for? Please [file an issue](https://github.com/18F/site-scanning/issues) or add your idea [to the list of proposed future scans](https://github.com/18F/site-scanning-documentation/blob/main/about/roadmap.md)!_
