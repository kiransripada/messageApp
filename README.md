# message-app

a [Sails v1](https://sailsjs.com) application

# Setup
+ Install Sails.js (it's to Node.js ...): sudo npm install sails -g
+ Create the application: sails new messageApp && cd messageApp
+ Create the message api: sails generate api message
+ Launch the application: sails lift

# Tests
+ Create new messages

+ curl -XPOST http://localhost:1337/message?text=hello
+ curl -XPOST http://localhost:1337/message?text=hola
+ Get list of messages

curl http://localhost:1337/message

[
 {
   "text": "hello",
   "createdAt": "2015-11-08T13:15:15.363Z",
   "updatedAt": "2015-11-08T13:15:15.363Z",
   "id": "5638b363c5cd0825511690bd"
 },
 +
 {
   "text": "hola",
   "createdAt": "2015-11-08T13:15:45.774Z",
   "updatedAt": "2015-11-08T13:15:45.774Z",
   "id": "5638b381c5cd0825511690be"
 }
]
+ Modify a message

curl -XPUT http://localhost:1337/message/5638b363c5cd0825511690bd?text=hey
+Delete a message

curl -XDELETE http://localhost:1337/message/5638b381c5cd0825511690be

### Links

+ [Sails framework documentation](https://sailsjs.com/get-started)
+ [Version notes / upgrading](https://sailsjs.com/documentation/upgrading)
+ [Deployment tips](https://sailsjs.com/documentation/concepts/deployment)
+ [Community support options](https://sailsjs.com/support)
+ [Professional / enterprise options](https://sailsjs.com/enterprise)


### Version info

This app was originally generated on Fri Apr 17 2020 15:07:21 GMT-0400 (EDT) using Sails v1.2.4.

<!-- Internally, Sails used [`sails-generate@1.16.13`](https://github.com/balderdashy/sails-generate/tree/v1.16.13/lib/core-generators/new). -->



<!--
Note:  Generators are usually run using the globally-installed `sails` CLI (command-line interface).  This CLI version is _environment-specific_ rather than app-specific, thus over time, as a project's dependencies are upgraded or the project is worked on by different developers on different computers using different versions of Node.js, the Sails dependency in its package.json file may differ from the globally-installed Sails CLI release it was originally generated with.  (Be sure to always check out the relevant [upgrading guides](https://sailsjs.com/upgrading) before upgrading the version of Sails used by your app.  If you're stuck, [get help here](https://sailsjs.com/support).)
-->

# messageApp
