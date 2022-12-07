# Social Media App

## Real time

Supabase hands us a lot of fun toys to make apps great. Add realtime updates and/or image uploads to your social media site, either as a group, or feel free to make a fork and work individually.

By no means should you limit yourselves to just the ideas listed below--be creative and have fun! This is all about getting ideas for project week.

That said, here are some sample ideas:

-   Make new messages from other users live update in the profile page
-   Add a chat room where all users can chat together at the same time
-   Make a game where users can see avatars walking around

---

Here is a sample schema for the `messages` table:

![image](https://user-images.githubusercontent.com/16160135/149589064-98af21ec-3d08-4891-80f1-d871e5581c7b.png)
Note that `recipient_id` is the id of the profile belonging to the recipient, _not_ the user_id

## Rubric

| Base Expectations                                                  |     |
| :----------------------------------------------------------------- | --: |
| Implement Supabase Real Time capability with your social media app |   5 |

| Functions                                                                                                                                                                              |     |
| :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --: |
| PURE: a render function that returns a DOM element (example: `renderMessagesEl(profile)` : takes in profile and returns a DOM element with all messages appended)                      |   3 |
| ASYNC: create a row in a supabase table (example: `sendMessage(message)` : takes in message object `{ sender_email_address, recipient_id, text }` and creates the message in supabase) |   2 |
