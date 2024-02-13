### Change Synology default ports of 443 and 80 to something else.

### Run the following commands:
This changes port 80 to port 82 as well as port 443 to 444. This allows the use of reverse proxies on Synology such as Traefik or NPM <br>
`sed -i -e 's/80/82/' -e 's/443/444/' /usr/syno/share/nginx/server.mustache /usr/syno/share/nginx/DSM.mustache /usr/syno/share/nginx/WWWService.mustache` <br>
<br>
`synosystemctl restart nginx`
