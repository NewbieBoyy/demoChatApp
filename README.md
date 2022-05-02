# Project title 
Demo Chat app using Io socket

# Documentation
https://www.tutorialspoint.com/socket.io/socket.io_quick_guide.htm .


lets say you are building a chat application user A on PC A or on his mobile phone sends a message to user B now there are sharing the same device they might be in two tottaly different place on the world Now user A sends a request to the server that contanis the message and the server store the messag in the database and the servver can return a response to user A but user B the person with whom user A chats does not send a request to hte server asking for the message or at least that is unlikely to happen, you could certainly use some pattern where you send a request every second to see if there are new messages but you will then hammer your sever with requests where most requests will not yield new messages so instead it would be nice to have some pish way of informing user b about the new message and that is exactly the scenario we are looking at here what is something changed on the server and we actively want to inform a client ? well then we can use wen socket instead of http
http is where we send a request and we get a response , web socket build up on http they are established via http, tbey use a so called http handshake to upgrade the htttp protocol to the web socket protocol and the web  scoket protocol that simply talks about how data is exchanged so this protocol is something you dont have to manage activelt the browser and the server communicate through a protocol and the used protocol define how the communication can happen with http it's reqeuest respomse ,with web sockets it's push data or actually both we can also send data from the client to the server this is still included but most importantly we can push data from the server to the client and you can and you typicaly will use both together in one and the same node-app so its not liek you have to decide do i build an app with web socket or do a build one with http you still have a lot pf place where you want to use that request response pattern for example if you are sending a message or if you are creating a user these are operation where you do send some information from the beowser to the server so ther ethe request response scenario make perfect sense but if you have some  actuve notification you want to get to your users then you also want to integrate web sockets
one of the most popular packages however is socket.io is a package that uses web scokets  and gives you a lot  of convenience features around that protocol that make it very easy to set up a web socket channel but with a client in the server and to use that cahnnel you can learn all about it her e in the offical  use the web scoket technoilogy the web scoket protocol and sets it up behind the scene for you you dont have to use socket.ip to use web scoket though you could one of the other options i showed 
##
![App Screenshot](https://tse1.mm.bing.net/th?id=OIP.-RYnmzf_nL4xRW41lf94NAHaF_&pid=Api&P=0&w=210&h=170)



# Tech Stack
Node,Express,IoSocket(library)

# Demo
https://www.crowdbotics.com/blog/build-chat-app-with-nodejs-socket-io

## Deployment
```bash
  npm init 
```
To run it 
```bash
  npm start
```

