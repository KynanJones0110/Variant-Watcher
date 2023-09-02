# Variant-Watcher

(Testing with data ingestion, due URLhaus' API only containing up to 3 days worth of entries, it seemed more appropriate (and going of Splunk's example) to utilize their 90 day dataset of URLs which come with tags to link them to associated variants, RedLine for example.

https://urlhaus-api.abuse.ch/
Notebook to aggregate data from a target Malware Variant. Currently, this is purely from URLhaus' dataset, the intention is to get as much data for the variant in question as possible, which will definitely require a total rework. This is my first project using Jupyter and really dabbling with anything like this using Python.

For now, it will aggregate a count of domains seen (top 20) from a variant.

Issues - Naming conventions, such as 'Red Line' -> 'RedLine' if present, will skew results. Will look at formatting the data prior to user input.
# To do

- Add in relevant API calls to pull info in general. (Possible just strip out core logic and rework and utilize this as a 90 day datset parser)
- Add in filter to specify what family/variant you would like to request IOCs on such as 
- Inputting Redline = 
-   Pulls top domains seen in last x days
-   Pulls top IPs seen in last x days
-   Pulls top hashes/file IOC seen in last x days (another dataset req)

Test with free APIs, malbaz, haus etc.
Test with multiple and format the data as required.

Massive inspiration taken from Splunk's Threat Hunting Team's JN:
https://www.splunk.com/en_us/blog/security/do-not-cross-the-redline-stealer-detections-and-analysis.html

