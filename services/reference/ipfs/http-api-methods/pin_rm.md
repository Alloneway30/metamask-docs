import Tabs from "@theme/Tabs";
import TabItem from "@theme/TabItem";

# `pin_rm`

## `/api/v0/pin/rm`

Remove pinned objects from local storage.

### Request

<Tabs>
  <TabItem value="Syntax" label="Syntax" default>

```bash
curl "https://ipfs.infura.io:5001/api/v0/pin/rm?arg=<ipfs-path>" \
  -X POST \
  -u "<YOUR-API-KEY>:<YOUR-API-KEY-SECRET>"
```

  </TabItem>
  <TabItem value="Example" label="Example" >

```bash
curl "https://ipfs.infura.io:5001/api/v0/pin/rm?arg=QmfQ5QAjvg4GtA3wg3adpnDJug8ktA1BxurVqBD8rtgVjM" \
  -X POST \
  -u "<YOUR-API-KEY>:<YOUR-API-KEY-SECRET>"
```

  </TabItem>
</Tabs>

#### Request parameters

- `arg` _\[Required]_ - Path to objects to be unpinned.

### Response

On success, the call to this endpoint returns with 200 and the following body:

#### Body

```
{
  "Pins": [
    "string"
  ]
}
```
