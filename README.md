# Commerce News Desk — public outputs

Three files the pipeline writes on every run, served for the site to fetch:

| File | What it is |
|---|---|
| `status.json` | Stories today, sources watched, last crawl, pipeline health. The Desk status component on commercenewsdesk.com reads this. |
| `feed.xml` | RSS 2.0, the newest 50 published briefs. |
| `ticker.json` | The last 12 headlines with desk and time. |

Written by [`solaracontent/commercenewsdesk`](https://github.com/solaracontent/commercenewsdesk), which is private and stays that way: its SQLite store holds the full body text of scraped articles, and the desk's conduct policy is that body text is read by the pipeline and never republished. This repository holds these three files and nothing else.

Do not edit by hand — every pipeline run overwrites them.
