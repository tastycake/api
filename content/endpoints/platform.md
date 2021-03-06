+++
date = "2017-01-11T20:46:03+10:00"
toc = true
next = "/endpoints/player-perspective"
prev = "/endpoints/person"
weight = 11
title = "Platform"

+++

***URL path:*** /platforms/

***Example response***

```json
{
    "id": 2,
    "name": "Point-and-click",
    "slug": "point-and-click",
    "url": "https://www.igdb.com/genres/point-and-click",
    "created_at": 123456789,
    "updated_at": 123456789,
    "games": [
      1,
      2,
      3,
      ...
    ]
}
```

***Fields***

| Name             | Type                              | Mandatory | Comment |
| ---------------- |:---------------------------------:|:---------:| ------- |
| id               | unsigned 64-bit integer           |     +     ||
| name             | string                            |     +     ||
| slug             | string                            |     +     ||
| url              | string                            |     +     ||
| created_at       | 64-bit integer                    |     +     | Unix epoch |
| updated_at       | 64-bit integer                    |     +     | Unix epoch |
| logo             | object                            |     -     | See the [Image](../../misc-objects/image) object reference |
| website          | string                            |     -     ||
| summary          | text (long string)                |     -     ||
| alternative_name | string                            |     -     ||
| generation       | integer                           |     -     ||
| games            | array of unsigned 64-bit integers |     -     | IDs of [Game](../game) records |
| versions         | array of objects                  |     -     | See the [Platform version](../../misc-objects/platform-version) object reference |

***Unused fields***

These fields are present in the meta field list but has no data for any of the entities.

| Name |
| ---- |
| shortcut |
| category |
| product_family 
|