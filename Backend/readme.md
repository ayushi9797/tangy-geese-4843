API endpoints
<!-- To start the server "npm start "-->
NO need to give token . Taken care by redis.cliet.Get
***
# register
localhost:8080/register
-name
-email
-pass
-pic link
# login
localhost:8080/login
-email
-pass

1.***To Get All Users data
localhost:8080/user/

2.***To get data user by search

localhost:8080/user?search={name/email}

# Message Section (Individual)
<!-- Message Route -->

<!-- 1.Sending a Message Route -->
localhost:8080/message/
-POST request


<!-- 2.To get all chat in that room -->
-GET request

localhost:8080/message/:chatId


# Group Chat
<!--Access The Chat  -->

1.get All chat
localhost:8080/chat
-post

2.get all chat
localhost:8080/chat
-GET

<!-- 3.Create A group Chat -->
localhost:8080/chat/group
<!-- Need to provide -->
-name of Group
-add members

<!-- 4.Rename The Group -->
localhost:8080/chat/renameGroup
<!-- Need to provide -->
-chatId i.e. group ID
- new Name

<!-- 5.remove Member from Group -->
localhost:8080/chat/removeFromGroup
<!-- Need to provide -->
-chatId of group
-userId of member

<!-- 6.add Member from Group -->
localhost:8080/chat/addToGroup
<!-- Need to provide -->
-chatId
-_id of member