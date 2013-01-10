Get statistics and revenues with our reporting API
==========================
Our reporting API allows you to get statistics for your account, for your ad space or ad campaign.

**Contents:**
* [Step 1 - Call function](#step-1---call-function)
* [Step 2 - Report parameters](#step-2---report-parameters)


# Step 1 - Call function:

**Example URL:**

https://plus1-report.wapstart.ru/client_type/report_type/object_id/?x-plus1-token&period=&group=&reportName=&dataType=

**client_type:**

Allows to use two different functions, publisher for publishers and advertiser for advertisers.

**report_type:**

Allows to use two different functions, common for the statistics and revenues and traffic for traffic data.

**object_id (optional):**

ID of your ad space or ad campaign. If not specified, will show the data for all ad spaces/ad campaigns.

**x-plus1-token:**

40 symbols auth key. You should contact client support to get the auth key (clientsupport@co.wapstart.ru).

**Note:** you can send x-plus1-token through GET, but we recommend to transfer the value through the same name of http header.


# Step 2 - Report parameters:

**period:**

1 – user period (has 2 parameters, beginDate and endDate in YYYY-MM-DD)

**Note:** if you select user period, beginDate and endDate will be required.

3 – today

4 – yesterday

100 – week

102 – month

9 – total

**group:**

(groups the data by time, only for common)

1 – hourly

2 – daily

3 – weekly

4 – monthly

5 – without group (sum of the results for the whole period)

**reportName:**

(type of the traffic report)

0 – carriers

1 – brands

2 – countries

3 – OS

4 – browsers

**dataType:**

jsonData – JSON

xmlData – XML
