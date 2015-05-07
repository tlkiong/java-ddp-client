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

To-Do
-----
* Update the current code
* Update this READ.ME
* Create a javadoc
