### Change Synology default ports of 443 and 80 to something else.

### Run the following commands:
Replace 82 with the port you want to change port 80 to and replace 444 with the new port for 443 <br>
`sed -i -e 's/80/82/' -e 's/443/444/' /usr/syno/share/nginx/server.mustache /usr/syno/share/nginx/DSM.mustache /usr/syno/share/nginx/WWWService.mustache` <br>
<br>
`synosystemctl restart nginx`
