Documentation of Group 7 (Social Media Platform):

- Rohaan Renu John
- Ankit Garai
- Kanakam Harika
- Nishant M
- Eragam Reddy Yashaswini


In our project we have implemented these entities as part of the backend for the social media platform in the Social_Media database:

- User_Table
- Post
- Comments
- Likes
- Replies
- user_group_membership
- user_group_follow

The API endpoints we have created are:



localhost:8080/api/v1/register - This is used to register a new user. They have to create enter their email, password and other details in order to successfully register into the database. The method here we use is the POST method.
Example JSON body for the register endpoint:
{
  "firstName" : "John",
  "lastName" : "Doe",
  "email" : "john.doe@gmail.com",
  "password" : "johndoe123",
  "matchingPassword" : "johndoe123",
  "role" : "USER"
}

localhost:8080/api/v1/login - This is used to login the user. If the username and password is correct then the user will be successfully registered. The method here we use is the POST method.
Example JSON body for the login endpoint:
{

  "username" : "john.doe@gmail.com",
  "password" : "johndoe123"

}



localhost:8080/api/v1/posts - This is used to create a new post. There should be the required post details in order to create a post successfully. The method here we use is the POST method. Here the auth token after successful verification needs to be mentioned as well in order for a successful request.
Example JSON body for the endpoint:
{
 "authorId" : 1,
 "postType" : "Text"
}









localhost:8080/api/v1/replies - This is used to create a new reply. There should be the required reply details in order to create a reply successfully. The method here we use is the POST method. Here the auth token after successful verification needs to be mentioned as well in order for a successful request.
Example JSON body for the endpoint:
{
 "replyId" : 1,
 "parentCommentId" : 1,
 "replyType" : "Text"
}





localhost:8080/api/v1/comments - This is used to create a new comment. There should be the required comment details in order to create a comment successfully. The method here we use is the POST method. Here the auth token after successful verification needs to be mentioned as well in order for a successful request.
Example JSON body for the endpoint:
{
 "commentId" : 1,
 "postId" : 1,
 "commenterId: 1,
 "commentText": "Hello",
 "typeOfComment": "Text"
}






localhost:8080/api/v1/likes - This is used to create a new like. There should be the required like details in order to create a like successfully. The method here we use is the POST method. Here the auth token after successful verification needs to be mentioned as well in order for a successful request.
Example JSON body for the endpoint:
{
 "likeId" : 1,
 "likedOnId": 1,
 "likeOnType": "Text",
 "likeById": 1,
 "reactionType": "Laugh"
}




localhost:8080/api/v1/user_group_membership - This is used to create a new group membership. There should be the required user group membership details in order to create a user group membership successfully. The method here we use is the POST method. Here the auth token after successful verification needs to be mentioned as well in order for a successful request.
Example JSON body for the endpoint:
{
 "userId" : 1,
 "joinedGroupOn" : "01-01-2020",
 "leftGroupOn" : "02-02-2020",
 "activeOrPassiveMember" : "False"
}






localhost:8080/api/v1/user_page_follow - This is used to create a new user page follow. There should be the required user page follow details in order to create a user page follow successfully. The method here we use is the POST method. Here the auth token after successful verification needs to be mentioned as well in order for a successful request.
Example JSON body for the endpoint:
{
 "userId" : 1,
 "joinedGroupOn" : "01-01-2020",
 "leftGroupOn" : "02-02-2020",
 "activeOrPassiveMember" : "False"
}



































































































































