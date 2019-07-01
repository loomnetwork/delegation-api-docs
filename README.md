# delegation-api-docs

# Delegation API

## Base URL

```
https://loom.games/api/delegation
```

## Endpoints

| Method        |  URL | Description |
| :-------------| :-----| :------- |
| `GET` | ```transaction``` | List delegation transaction order by block number |
| `GET` | ```total``` | List total delegation order by timestamp |
| `GET` | ```validator``` | List total delegation group by validator order by timestamp |


## GET /transaction

**Optional filter parameters:**

| Name        |  Type |
| :-----------| :-----|
| delegator | string |
| validator | string |
| state | string |
| lock_time_tier | string |
| from_block | number |
| to_block | number |

**Response**

```
{
  "data": [
    {
      "id": 4498,
      "created_at": "2019-03-12T09:23:34Z",
      "updated_at": "2019-03-12T09:23:35Z",
      "delegator": "default:0x509f262395d7Eae18E059bfa3Cb5CdF5f7D15faC",
      "validator": "default:0xac3211caEcc45940A6D2BA006ca465A647d8464F",
      "update_validator": "",
      "amount": "10000000000000000000",
      "update_amount": "",
      "block_height": 1763986,
      "lock_time": 1547813218,
      "lock_time_tier": "TIER_ZERO",
      "state": "BONDED",
      "lock_time_at": "2019-01-18T12:06:58Z"
    },
    {
      "id": 3807,
      "created_at": "2019-03-12T09:23:34Z",
      "updated_at": "2019-03-12T09:23:34Z",
      "delegator": "default:0x06926a2cdC99fFaaFc406Cd34092235D7376131b",
      "validator": "default:0x2A3a7C850586d4F80A12ac1952f88B1b69ef48E1",
      "update_validator": "",
      "amount": "30000000000000",
      "update_amount": "",
      "block_height": 2144898,
      "lock_time": 1580279105,
      "lock_time_tier": "TIER_ZERO",
      "state": "BONDED",
      "lock_time_at": "2020-01-29T06:25:05Z"
    },
    {
      "id": 4491,
      "created_at": "2019-03-12T09:23:34Z",
      "updated_at": "2019-03-12T09:23:35Z",
      "delegator": "default:0x06926a2cdC99fFaaFc406Cd34092235D7376131b",
      "validator": "default:0xac3211caEcc45940A6D2BA006ca465A647d8464F",
      "update_validator": "",
      "amount": "340000102000000000",
      "update_amount": "",
      "block_height": 2145515,
      "lock_time": 1580280636,
      "lock_time_tier": "TIER_THREE",
      "state": "BONDED",
      "lock_time_at": "2020-01-29T06:50:36Z"
    },
    {
      "id": 4262,
      "created_at": "2019-03-12T09:23:34Z",
      "updated_at": "2019-03-12T09:23:35Z",
      "delegator": "default:0x06926a2cdC99fFaaFc406Cd34092235D7376131b",
      "validator": "default:0xa38c27e8Cf4a443E805065065Aefb250b1E1cef2",
      "update_validator": "",
      "amount": "10000000000000",
      "update_amount": "",
      "block_height": 2147085,
      "lock_time": 1548748731,
      "lock_time_tier": "TIER_ZERO",
      "state": "BONDED",
      "lock_time_at": "2019-01-29T07:58:51Z"
    }
}
```

## GET /total

**Optional filter parameters:**

| Name        |  Type |
| :-----------| :-----|
| from_date | date |
| to_date | date |


**Response**

```
{
  "data": [
    {
      "id": 45,
      "created_at": "2019-03-13T10:37:48Z",
      "updated_at": "2019-03-13T10:37:48Z",
      "delegationTotal": "56032841669040102002000000"
    },
    {
      "id": 54,
      "created_at": "2019-03-13T10:42:17Z",
      "updated_at": "2019-03-13T10:42:17Z",
      "delegationTotal": "56032841669040102002000000"
    },
    {
      "id": 92,
      "created_at": "2019-03-13T14:07:51Z",
      "updated_at": "2019-03-13T14:07:51Z",
      "delegationTotal": "56062035389040102002000000"
    },
    {
      "id": 118,
      "created_at": "2019-03-13T16:17:50Z",
      "updated_at": "2019-03-13T16:17:50Z",
      "delegationTotal": "56062798269040102002000000"
    },
    {
      "id": 137,
      "created_at": "2019-03-13T17:52:49Z",
      "updated_at": "2019-03-13T17:52:49Z",
      "delegationTotal": "56063880269040102002000000"
    },
    {
      "id": 151,
      "created_at": "2019-03-13T19:02:50Z",
      "updated_at": "2019-03-13T19:02:50Z",
      "delegationTotal": "56063880269040102002000000"
    },
    {
      "id": 172,
      "created_at": "2019-03-13T20:47:50Z",
      "updated_at": "2019-03-13T20:47:50Z",
      "delegationTotal": "56066209389040102002000000"
    },
    {
      "id": 180,
      "created_at": "2019-03-13T21:27:50Z",
      "updated_at": "2019-03-13T21:27:50Z",
      "delegationTotal": "56125219389040102002000000"
    },
    {
      "id": 193,
      "created_at": "2019-03-13T22:32:50Z",
      "updated_at": "2019-03-13T22:32:50Z",
      "delegationTotal": "56130544389040102002000000"
    },

```

## GET /validator

**Optional filter parameters:**

**Optional filter parameters:**

| Name        |  Type |
| :-----------| :-----|
| validator | string |
| from_date | date |
| to_date | date |

**Response**

```
{
  "data": [
    {
      "id": 630,
      "created_at": "2019-03-14T06:49:48Z",
      "updated_at": "2019-03-14T06:49:49Z",
      "delegationTotal": "251977770000000000000000",
      "validator": "default:0xeB5d1FA6E421485C7ae2fbA8E3199588eD931dAf"
    },
    {
      "id": 645,
      "created_at": "2019-03-14T06:50:48Z",
      "updated_at": "2019-03-14T06:50:49Z",
      "delegationTotal": "251977770000000000000000",
      "validator": "default:0xeB5d1FA6E421485C7ae2fbA8E3199588eD931dAf"
    },
    {
      "id": 660,
      "created_at": "2019-03-14T06:51:48Z",
      "updated_at": "2019-03-14T06:51:49Z",
      "delegationTotal": "251977770000000000000000",
      "validator": "default:0xeB5d1FA6E421485C7ae2fbA8E3199588eD931dAf"
    },
    {
      "id": 675,
      "created_at": "2019-03-14T06:52:48Z",
      "updated_at": "2019-03-14T06:52:49Z",
      "delegationTotal": "251977770000000000000000",
      "validator": "default:0xeB5d1FA6E421485C7ae2fbA8E3199588eD931dAf"
    }
  ]
}
```
