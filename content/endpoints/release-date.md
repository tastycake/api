+++
date = "2017-01-15T17:38:45+10:00"
toc = true
next = "/endpoints/review"
prev = "/endpoints/pulse"
weight = 14
title = "Release date"

+++

***URL path:*** /release_dates/

***Example response***

```json
{
    "id": 4034,
    "game": 1936,
    "category": 7,
    "platform": 48,
    "human": "TBD"
}
```

***Fields***

| Name     | Type                    | Mandatory | Comment |
| -------- |:-----------------------:|:---------:| ------- |
| id       | unsigned 64-bit integer |     +     ||
| game     | unsigned 64-bit integer |     +     | ID of a [Game](../game) record |
| category | unsigned integer        |     +     | See the [Date category](../../enum-fields/date-category) value reference |
| platform | unsigned 64-bit integer |     +     | ID of a [Platform](../platform) record |
| human    | string                  |     +     | The release date in human readable format. |
| updated_at | 64-bit integer        |     +     | When the release_date was updated. |
| created_at | 64-bit integer        |     +     | When the release_date was created. |
| date     | 64-bit integer          |     -     | Unix epoch |
| region   | unsigned integer        |     -     | ID of a [Region](../region) |
| y        | unsigned integer        |     -     | The year in 4-digit format |
| m        | unsigned integer        |     -     | The month in no-leading-zero format (1-12) |

***Unused fields***

These fields are present in the meta field list but has no data for any of the entities.

| Name |
| ---- |
| region |