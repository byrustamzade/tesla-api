# Software Updates

## POST `/api/1/vehicles/{id}/command/schedule_software_update`

Schedules a software update to be installed, if one is available.

### Parameters

| Parameter  | Example | Description                                                                            |
| :--------- | :------ | :------------------------------------------------------------------------------------- |
| offset_sec | 7200    | How many seconds in the future to schedule the update. Set to 0 for immediate install. |

### Response

```json
{
  "reason": "",
  "result": true
}
```

## POST `/api/1/vehicles/{id}/command/cancel_software_update`

Cancels a software update, if one is scheduled and has not yet started.

### Response

```json
{
  "reason": "",
  "result": true
}
```
