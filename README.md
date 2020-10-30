# ATL City Council Scraper

https://citycouncil.atlantaga.gov/ is the authoritative source for Atlanta City Council information.

This repository scrapes council member info into JSON for consumption by apps and APIs.

Scraping is done daily via Github Actions. Neat technique.<sup>[1](https://simonwillison.net/2020/Oct/9/git-scraping/)</sup>

Get the most recent [scraped data here](scraped/atl-citycouncil.json).

For self-hosting you have two options:

## Run in a container

`docker run abriedev/atl-council-scraper scrape`

## Build from source

__Requires Python 3.8__

1. `make dependencies`
2. `make test`
3. `python3 -m app scrape`
