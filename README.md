Meteor.js Java DDP Client
=========================

Origins/Acknowledgements
------------------------
This is a fork from [Ken Yee' 
DDP Client](https://github.com/kenyee/java-ddp-client)
which is a fairly big fleshing out of [Peter Kutrumbos' 
DDP Client](https://github.com/kutrumbo/java-ddp-client).

Differences include:
* Reconnection - number of reconnection before close connection & delay time before retry connection
* SSL & Trust Manager Working for reconnet
* Handle onChanged message from DDP Collection
* Handle resend message for reconnection
* Must have an error listener to listens for all errors

Take Note
-----
* Meteor server disconnect and have to "Relogin". Might have weird response
* Since there is reconnection, there might appear a case where the server DC and then the client will reconnect and then server DC again.
** Thus, there will be a loop on the DC -> RC which WILL consume resources and hang the application

To-Do
-----
* Update the current code
* Update this READ.ME
* Create a javadoc
