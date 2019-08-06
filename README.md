# Breakdown-Merged-AssetID
Reports downloaded from CMS alwasy have merged Asset IDs in the column "asset id". This python scrip is designed for breaking down multiple asset ids in one cell to multiple cells

Eg, this is the table before running the code

| Asset ID | Views | Revenue |
| ------------- | ------------- | ------------- |
| A\|B\|C  | 33  | 66  |
| B\|D  | 50  | 90  |

Run this table with this code, you will get the table:

| Asset ID | Views | Revenue |
| ------------- | ------------- | ------------- |
| A  | 11 | 22  |
| B  | 11  | 22  |
| C  | 11  | 22  |
| B  | 25  | 45  |
| A  | 25  | 45  |

PLEASE BE NOTIFED, the table format you use the table would be:
1. The first column would always be the merged asset ids you want to break down
2. Any column after the first column would only be numerical because there are the numbers are going to be average.
Baseically the table format should be like this:

| Asset ID | Views | Revenue | ....
| ------------- | ------------- | ------------- | ------------- |
| A\|E  | 11 | 22  | .....
