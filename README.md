# Home Server

This is a dockerized home server setup. It will allow you to be up and running
very quickly without having to worry about installing each component. The only
thing you should need to do is make sure the directories are in place,
configure the programs, and (optionally) set up port forwarding on your router

## Included programs

### Transmission

[Transmission](https://transmissionbt.com/) is a simple BitTorrent client that
is used to download torrents. The other programs can connect to it to add new
torrents or you can add them manually.

### Sonarr

[Sonarr](https://sonarr.tv/) is an interface for managing TV series. It
connects to a download client, like Transmission to download them or it can
also find existing ones on the file system.

### Radarr

[Radarr](https://radarr.video/) is like Sonarr but for Movies. It can use a
download client or find existing movies on the file system.

### Lidarr

[Lidarr](https://lidarr.audio/) is for music what Sonarr and Radarr are for TV
and movies.

### Jackett

[Jackett](https://github.com/Jackett/Jackett) acts as an API endpoint for
torrent trackers. You can add them to Jackett and then have Sonarr and Radarr
connect to the Jackett endpoint for the searching.

### Plex

[Plex](https://www.plex.tv) will be your interface for actually playing the
media that you're managing via the previously-listed components.