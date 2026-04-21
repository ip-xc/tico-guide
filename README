# tico-guide
<!-- Tagline -->
tico is the first custom emulation frontend for Nintendo Switch - a controller-first, native C++ interface designed for performance, simplicity, and long-term portability.

This guide tries to be as hands-on as possible and cover most questions along the way.

<!-- Table of Contents -->
<p align="center">
  <a href="#about">About</a> •
  <a href="#prerequisites">Prerequisites</a> •
  <a href="#deployment">Deployment</a> •
  <a href="#usage">Usage</a> •
  <a href="#credits">Credits</a> •
</p>

## About
This is a small guide that helps you start a small media server on your local network, incorperating local files stored on your Synology NAS and using the Gelato plugin to fetch media with your debrid account.

For further details about tico, please visit their [Github repository](https://github.com/ticohq/tico).

| :warning: At the time of this guide I am running HOS 22.1.0 and tico 0.7.0. This guide might be subject to change. |
| --- |

## Prerequisites 

* **A compatible Nintendo Switch** --> please refer to one of the dozens of setup guides to see the supported models (V1, Lite & OLED).
* A way to **write and modify files** on your Switch (MTP, FTP..).

## Deployment
1. First, download the **latest** Release of tico from [Github here](https://github.com/ticohq/tico/releases).

<div><img width="1024" src="placeholder" alt="first"> </div>

2. Connect to your Nintendo Switch and open the SD cards root folder "/".

<div><img width="1024" src="placeholder" alt="second"></div>

3. **Extract and copy** the files from "**tico-release.zip**" inside the "**SD card**".

<div><img width="1024" src="placeholder" alt="third"></div>

4. Press **"Next"** to start the project. When it's done running and created the container, you can visit your Jellyfin instance via **http://<IP_OF_NAS>:8096/**.

5. Create your Administrator and go to your admin overview to add a library for your movies and shows.

<div><img width="1024" src="/Guide/metadata.png" alt="metadata"></div>
<div><img width="1024" src="/Guide/shows_1.png" alt="shows"></div>

Do **NOT** use the folders containing your existing media for Gelato. Always create a new folder!

Also keep in mind, that for the Metadata downloaders, "**TheMovieDb**" should be **OVER** "**The Open Movie Database**".

6. Scan the library after adding the Gelato paths.

7. Install the Gelato plugin. Add the repository as a custom repository to Jellyfin. It takes up to 30 minutes to have the plugin show up as available.

```https://raw.githubusercontent.com/lostb1t/Gelato/refs/heads/gh-pages/repository.json```

<div><img width="1024" src="/Guide/4.png" alt="four"></div>

8. After installing Gelato, you have to configure the plugin. [Please refer to the Setup Guide by @lostb1t](https://github.com/lostb1t/Gelato/discussions/40)

## Credits
The Jellyfin-Team, for creating this awesome fork - [Github repository](https://github.com/jellyfin/jellyfin) or their [Website](https://jellyfin.org/).

lostb1t for creating Gelato, please visit their [Github repository](https://github.com/lostb1t/Gelato).
