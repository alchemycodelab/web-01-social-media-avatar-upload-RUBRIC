# web-01-social-media-avatar-upload-RUBRIC

## Part A

Here is a sample schema for the `profiles` table:

![profiles table- column names and types](/assets/profiles-table.png)

### Live Example:

https://miniature-spoon-7bbe0953.pages.github.io/

| Events                                                                                                                                                                         |     |
| :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --: |
| On the profiles page load, fetch the profiles from supabase and render them to the page. Each profile should contain a link to that profile's detail page (using query params) |   2 |
| On the profile detail page load, use the query param to fetch the correct profile and display the email or username of the profile to the user                                 |   2 |
| On the profile detail page load, display the popularity of the user                                                                                                            |   2 |
| On the profile detail page, when the user upvotes or downvotes the profile, the popularity is updated correctly and displayed to the user                                      |   4 |

| Functions                                                                                                                                                                                 |     |
| :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --: |
| PURE: `renderPopularityEl(profile)` : takes in profile and returns a DOM element with karma and buttons (with event listeners to increment and decrement karma)                           |   1 |
| ASYNC: `upsertProfile()` : creates or updates a profile in supabase                                                                                                                       |   2 |
| ASYNC: `getProfile(id)` : takes in id and returns profile with matching id, including its related messages                                                                                |   1 |
| ASYNC: `incrementPopularity(id) and decrementPopularity(id)` : takes in id of profile to update, fetches that profile to find current Popularity, then updates that profile appropriately |   1 |
