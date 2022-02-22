# Cthulhu

Cthulhu is a simple python CLI application that facilitates the streaming of torrents directly from various sources. It uses [peerflix](https://github.com/mafintosh/peerflix) to stream video from magnet links directly.

<p align="center">
<img src="./preview.gif" alt="Video Preview" width="700px">
</p>

Cthulhu is heavily inspired by [Bugswriter's notflix](https://github.com/Bugswriter/notflix), which was written using shell scripting. The differences between our programs aren't very stark. All in all, I wrote this program mainly for fun and practice. 

Feel free to submit issues and feature requests.

### Notable Features (so far)

- Runs directly from the terminal
- macOS and BSD support (theoretical, needs testing)
- multiple source options (currently: 1337x, nyaa)
- Ability to list multiple files in a torrent (useful for binging TV shows)
- Filtering out unwanted results by default, such as application files and pornogrophy

## Requirements

- [mpv](https://github.com/mpv-player/mpv) or [vlc](https://github.com/videolan/vlc)
- [requests](https://docs.python-requests.org/en/latest/) - A python library for making http requests. `pip3 install requests`
- [lxml](https://lxml.de/) - A python library for parsing XML/HTML. `pip3 install lxml`
- [peerflix](https://github.com/mafintosh/peerflix) - A tool to stream torrents. `npm install -g peerflix`

## Installation for Linux/macOS

### cURL

Make sure that `/usr/local/bin` exists with the proper permissions. If not, then `sudo mkdir -p -m 775 /usr/local/bin `

cURL **cthulhu** to your **$PATH** and give execute permissions.

```sh
sudo curl -sL "https://raw.githubusercontent.com/trianglecirclexyz/cthulhu/main/cthulhu" -o /usr/local/bin/cthulhu
sudo chmod +x /usr/local/bin/cthulhu
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, remove `cthulhu` from your **$PATH**, for example `sudo rm -f /usr/local/bin/cthulhu.`


