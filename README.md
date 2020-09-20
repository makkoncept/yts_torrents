# Thoughts on archiving

I am archiving this (and the related repositories - [yts.am_scraper](https://github.com/makkoncept/yts.am_scraper_) and [movie_torrents](https://github.com/makkoncept/movie_torrents)). There are several reasons but the most prominent one being that some people might use it for torrenting unsanctioned copyrighted material. As mentioned in the disclaimer, this was not the goal. Maybe this was the reason that I have not thought about this project since the time it was put on Github and therefore it's very outdated and might not even work out-of-the-box.

# yts_torrents

download all torrents from yts.am (yify movies). Uses yify api.

**Used to create [movie_torrents](https://github.com/makkoncept/movie_torrents)[repository of 10k+ movie torrents].**

## Usage

- clone the repo

```
git clone https://github.com/makkoncept/yts_torrents.git
cd yts_torrents
```

- Create a virtualenv:

```
python3 -m venv venv
```

- Activate it on Linux:

```
. venv/bin/activate
```

- Or on Windows cmd:

```
venv\Scripts\activate.bat
```

- Install requests

```
pip install requests
```

run `python yts_am_api.py` to make json files containing torrent links of the movies. Then run `python linkdownload.py`
to parse the created json files and download the torrents.

## Priority

The torrents will be downloaded according to the following priority:

1080p bluray> 1080p web> 720p bluray> 720p web

## Disclaimer

Downloading copyright movies may be illegal in your country. This tool is for educational purposes only and was created only to experiment with [yify api](https://yts.am/api)
