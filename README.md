# Markdown-Data
A way of incorporating data into markdown. Not sure if this is a great idea :\

## Example API endpoint
```
https://data.qld.gov.au/api/action/datastore_search?resource_id=6e4b863c-ceb4-4191-929e-adb74f5b64e3
```
### Output JSON
```json
{
    "help": "https://data.qld.gov.au/api/3/action/help_show?name=datastore_search",
    "success": true,
    "result": {
        "resource_id": "6e4b863c-ceb4-4191-929e-adb74f5b64e3",
        "fields": [],
        "records": [
            {
                "Status": "Indigenous",
                "Count": "13",
                "LGA Code": "30250",
                "Age": "0",
                "Sex": "F",
                "LGA Name": "Aurukun (S)",
                "Year": "2001",
                "_id": 1
            },
            {
                "Status": "Indigenous",
                "Count": "14",
                "LGA Code": "30250",
                "Age": "1",
                "Sex": "F",
                "LGA Name": "Aurukun (S)",
                "Year": "2001",
                "_id": 2
            },
            {
                "Status": "Indigenous",
                "Count": "9",
                "LGA Code": "30250",
                "Age": "2",
                "Sex": "F",
                "LGA Name": "Aurukun (S)",
                "Year": "2001",
                "_id": 3
            },
            {
                "Status": "Indigenous",
                "Count": "10",
                "LGA Code": "30250",
                "Age": "3",
                "Sex": "F",
                "LGA Name": "Aurukun (S)",
                "Year": "2001",
                "_id": 4
            }
        ],
        "_links": {
            "start": "/api/action/datastore_search?resource_id=6e4b863c-ceb4-4191-929e-adb74f5b64e3",
            "next": "/api/action/datastore_search?offset=100&resource_id=6e4b863c-ceb4-4191-929e-adb74f5b64e3"
        },
        "total": 140250
    }
}
```
## Usage
```
@(https://data.qld.gov.au/api/action/datastore_search?resource_id=6e4b863c-ceb4-4191-929e-adb74f5b64e3)<result/records>
```
### Output
<table>
<thead>
<tr>
<th>Status</th>
<th>Count</th>
<th>LGA Code</th>
<th>Age</th>
<th>Sex</th>
<th>LGA Name</th>
<th>Year</th>
<th>_id</th>
</tr>
</thead>
<tbody>
<tr>
<td>Indigenous</td>
<td>13</td>
<td>30250</td>
<td>0</td>
<td>F</td>
<td>Aurukun (S)</td>
<td>2001</td>
<td>1</td>
</tr>

<tr>
<td>Indigenous</td>
<td>14</td>
<td>30250</td>
<td>1</td>
<td>F</td>
<td>Aurukun (S)</td>
<td>2001</td>
<td>2</td>
</tr>

<tr>
<td>Indigenous</td>
<td>14</td>
<td>30250</td>
<td>2</td>
<td>F</td>
<td>Aurukun (S)</td>
<td>2001</td>
<td>3</td>
</tr>

<tr>
<td>Indigenous</td>
<td>14</td>
<td>30250</td>
<td>3</td>
<td>F</td>
<td>Aurukun (S)</td>
<td>2001</td>
<td>4</td>
</tr>
</tbody>
</table>
