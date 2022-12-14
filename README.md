# Social Media App

### Template

Begin with the [supabase-web-template](https://github.com/alchemycodelab/web-template-supabase)

## Part A: Profile page with Avatar Upload

Here is a sample schema for the `profiles` table:

![profiles table- column names and types](/assets/profiles-table.png)

| Events                                                                                                                                                                         |     |
| :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --: |
| On the profiles page load, fetch the profiles from supabase and render them to the page. Each profile should contain a link to that profile's detail page (using query params) |   2 |
| On the profile detail page load, use the query param to fetch the correct profile and display the email or username of the profile to the user                                 |   2 |
| On the profile detail page load, display the popularity of the user                                                                                                            |   2 |
| On the profile detail page, when the user upvotes or downvotes the profile, the popularity is updated correctly and displayed to the user                                      |   4 |
| Submit screenshots of your supabase table, policies, and bucket storage setup                                                                                                  |   4 |

| Functions                                                                                                                                                                                 |     |
| :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --: |
| PURE: `renderPopularityEl(profile)` : takes in profile and returns a DOM element with karma and buttons (with event listeners to increment and decrement karma)                           |   1 |
| ASYNC: `upsertProfile()` (or `createProfile()` and `updateProfile()`) : creates and updates a profile in supabase                                                                         |   2 |
| ASYNC: `getProfile(id)` : takes in id and returns profile with matching id, including its related messages                                                                                |   1 |
| ASYNC: `incrementPopularity(id) and decrementPopularity(id)` : takes in id of profile to update, fetches that profile to find current Popularity, then updates that profile appropriately |   1 |
| ASYNC: `uploadImage(imagePath, imageFile)` : takes in imagePath and imageFile and returns url to the image                                                                                |   1 |
