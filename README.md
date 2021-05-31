# Torrent-client
This project aims to build a bit torrent Client REST Api

#**Project details:**
Step 1: We send a request to a tracker, and the tracker will respond with a list of peers. More specifically, we tell the tracker which files we’re trying to download, and the tracker gives you the ip address of the users we download them from. Making a request to a tracker also adds our ip address to the list of users that can share that file.

Step 2: After we have the list of peer addresses, we connect to them directly and start downloading. This happens through an exchange of messages where they tell what pieces they have, and we tell them which pieces you want.


dingachika.torrent is the sample tracker file we used.


# src/tracker.js 
Need to increment index from 0 to the "index" whereever it works  and check the functionality in the 
Line : "const url = torrent["announce-list"][index].toString('utf8');"

# command to run code
 node index.js home/path_to_torrent_file
