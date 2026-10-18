
# slack-javascript

This [SDK](https://github.com/sdk-fabric/slack-javascript) is managed by the [SDK Fabric](https://sdk-fabric.org/) project, a global infrastructure to
automatically generate SDKs for every API.

You can find more information about this SDK at [TypeHub](https://typehub.cloud/):
https://app.typehub.cloud/d/sdkfabric/slack

## Usage

```typescript
const client = Client::build('[access_token]');

// Deletes a message from a channel.
const response = await client.chat().delete(new Delete_Message_Request());

// Retrieves a permalink URL for a specific existing message.
const response = await client.chat().getPermalink("channel", "message_ts");

// Sends an ephemeral message to a user in a channel.
const response = await client.chat().postEphemeral(new Post_Ephemeral_Request());

// Sends a message to a channel.
const response = await client.chat().postMessage(new Post_Message_Request());

// Schedules a message to be sent to a channel at a future time.
const response = await client.chat().scheduleMessage(new Schedule_Message_Request());

// Updates a message in a channel.
const response = await client.chat().update(new Update_Message_Request());
```
