# Supabase Messenger App

Here is a sample schema for the `messages` table:

![image](https://user-images.githubusercontent.com/16160135/149589064-98af21ec-3d08-4891-80f1-d871e5581c7b.png)

| Events                                                                                                                       |     |
| :--------------------------------------------------------------------------------------------------------------------------- | --: |
| On the profile detail page load, loop through and display the messages of the profile to the user                            |   2 |
| On the profile detail page, when the user sends a message, the message is created in supabase and then displayed to the user |   2 |

| Functions                                                                                                                                                                                                                                   |     |
| :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --: |
| PURE: `renderMessagesEl(profile)` : takes in profile and returns a DOM element with all messages appended                                                                                                                                   |   2 |
| ASYNC: `sendMessage(message)` : takes in message object `{ sender_email_address, recipient_id, text }` and creates the message in supabase. Note that `recipient_id` is the id of the profile belonging to the recipient, _not_ the user_id |   1 |
