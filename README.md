Key entities based on the user story:

Users: Store user profiles, followers, and following lists.
Posts: Store text, images, or videos with timestamps.
Likes: Track users who liked a post.
Comments: Store comments on posts.
Shares: Track post shares by users.



API Endpoints

1. User Endpoints

POST /api/users - Create a new user.

GET /api/users/{id} - Get a user’s profile details.

PUT /api/users/{id} - Update user profile.

POST /api/users/{id}/follow - Follow another user.

POST /api/users/{id}/unfollow - Unfollow a user.

2. Post Endpoints

POST /api/posts -  New post created.

GET /api/posts/{id} - Get details of a post.

GET /api/posts/user/{id} - Get posts by a user.

POST /api/posts/{id}/like - Like a post.

POST /api/posts/{id}/comment - Comment on a post.

POST /api/posts/{id}/share - Share a post.

3. Comment Endpoints

POST /api/comments -  comment on a post.

DELETE /api/comments/{id} - Delete a comment.

4. Follow Endpoints

POST /api/follow - Follow another user.

DELETE /api/follow - Unfollow a user.

5. Feed Endpoints

GET /api/feed/{user_id} - Get the feed for a user.