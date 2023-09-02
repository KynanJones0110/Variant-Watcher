# Variant-Watcher
![empise_Malware_Variant_Watcher_logo_f24b2355-522e-42da-8278-68cd0593c87b](https://github.com/KynanJones0110/Variant-Watcher/assets/71669145/1331fa53-9841-4e84-9295-0016e2898e69)

Notebook to aggregate data from a target Malware Variant. Currently, this is purely from URLhaus' dataset, the intention is to get as much data for the variant in question as possible, which will definitely require a total rework. This is my first project using Jupyter and really dabbling with anything like this using Python.

For now, it will aggregate a count of domains seen (top 20) from a variant.

Issues - Naming conventions, such as 'Red Line' -> 'RedLine' if present, will skew results. Will look at formatting the data prior to user input.
# To do

- Add in relevant API calls to pull info in general.
- Add in filter to specify what family/variant you would like to request IOCs on such as 
- Inputting Redline = 
-   Pulls top domains seen in last x days
-   Pulls top IPs seen in last x days
-   Pulls top hashes/file IOC seen in last x days (another dataset req)

Test with free APIs, malbaz, haus etc.
Test with multiple and format the data as required.

https://www.splunk.com/en_us/blog/security/do-not-cross-the-redline-stealer-detections-and-analysis.html
As seen below, and mentioned once or twice, heavy inspiration taken from Splunk's team:

<img width="439" alt="image" src="https://github.com/KynanJones0110/Variant-Watcher/assets/71669145/acde6faa-5750-4352-98f0-fa8274382d66">

