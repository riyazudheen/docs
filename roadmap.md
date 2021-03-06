# Development plans


* [Graphical user interface](#graphical-user-interface)
* [Data share](#data-share)
* [Distributed data rebuilding](#distributed-data-rebuilding)
* [Global search](#global-search)
* [Chat/Video/Conferencing](#chat/video/conferencing)
* [Decentralized Mail](#decentralized-mail)
* [Monetization through cryptocurrency](#monetization-through-cryptocurrency)
* [Anonymous logon](#anonymous-logon)
* [Decentralized social network](#decentralized-social-network)
* [Distributed WEB-hosting](#distributed-web-hosting)
* [Endless virtual worlds](#endless-virtual-worlds)


## Graphical user interface

Has already begun work on creating a visual user interface for BitDust software.

Interaction with the user will be implemented using a standard Internet browser,
which is present in almost any operating system.
A small WEB-server will be started at the begining of the program.
This will look like a "local" web site and use Django Framework to build visualized content for the user.

This way we can develop a lightweight and cross-platform user interface
and provide complete freedom for designer.



## Data share

This is one of the key steps that will allow users not only to store their own data 
in a completely secure environment, but also provide access to distributed data to other members 
of the network.

Will be implemented a model which is close to the classic POSIX-compliant platforms, 
where there are three levels of access to the file or directory: user, group, others. 

The user can set permissions to read/write any single folder or file in his distributed 
on the set of nodes storage.

This concept will provide many differnt features.
Imagine, if you posses appropriate permissions:

+ other users can download already uploaded data 
+ make changes, to work with shared files and folders
+ create a private distributed storage for groups of users
+ make safe and hidden transfers of data
+ create a fully shared and open data stores
+ safely distribute and advertise any data over the network
+ use the quick links for easy and safe delivery of data for single nodes
+ create endless storage



## Distributed data rebuilding

At this point in the BitDust software implemented a mechanism for automatic data rebuilding,
to be able to reconstruct a missing data segments when updating a lost supplier.
The whole process is fully automatic and does not require any actions from user in order
to maintain downloaded   data into the BitDust network.

Automatic rebuilding occurs on the data owner's node and requires constant work of BitDust
software on its machine and stable Internet connection.

Possible to transfer this functionality on other nodes that will support the downloaded data
to the network - we planned to call them "scrubbers".
The user can hire some number of scrubbers - they will consume system resources of their personal
computers to rebuild user's data on new suppliers.

An interesting feature of the proposed approach is that the scrubbers do not have access
to user's data, since they always operate with encrypted data.
This allows you to safely authorize to scrub your data to any nodes in the BitDust network 
and repeatedly increase storage reliability and speed up of uploading and downloading data.
The whole process of the remote automatic recovery will occur entirely without
the participation of the user. After downloading the data to the network,
you can shutdown your computer, or simply stop the BitDust software.

Together with the ability to share data, the implementation of this phase will make possible
to completely anonymous transmission and dissemination of data on the Internet.
Imagine, the owner of the data use a temporary IP address at first time he enters in the BitDust network
and made initial data uploading. Then he never use this identity file to enter the network again. 
This way his supplies actually will have no real information about him - it's like make a call
from a stolen SIM-card and throw it out.
His scrubbers thus will continue to engage in automatic restoring and maintaining downloaded data 
in the BitDust network, so that data stay  available for everyone.
Later, the owner of the data can go and download them using a different identity, this way
he will not be recognized.



## Global search

We would like to add a search engine in the BitDust software.
This should let users find a data in the global space which is granted a full read access - just
like a well-known torrents.
To any folder or file can be created and text description, on its base will be formed
list of key words which make up the global search index. 

In a few simple steps the owner of uploaded data can prepare the necessary information
and puts it into a global registry, which is stored into the distributed hash table.
Special "crawlers" sooner or later will visit the newly created topic,
validate it and make the appropriate changes in the global index.

This functionality will provide a completely safe and independent data distribution over 
the BitDust network, uncensored and possibility to exert any pressure on users by third parties.
This is a significant advantage in comparison with classical torrent trackers.
Their WEB sites are  under pressure from the copyright holders of content that is distributed there.



## Chat/Video/Conferencing

Has already been implemented simple functionality to transfer encrypted private messages between nodes.
They are transmitted directly from sender to receiver, protected with digital signature of the sender
and encrypted with secret key of recipient before sending it to the network.

In parallel with the development of the graphical user interface, will be developed a methods
for simple exchange of short messages just like in a typical chat system.
The history can be stored on user's suppliers so can be accessible at any time.

We planned also to introduce a streaming voice and video transmission
and implement a fully distributed and safe conferencing.



## Decentralized Mail

It would be convenient to provide users with a familiar environment for the conduct of personal 
correspondence.
It is proposed to use a  mail SMTP / POP3 / IMAP client, which the user  usual uses for 
transmitting/receiving e-mails.
This does not require to install anything else.

In the BitDust software has already been implemented a basic functionality for direct transfer 
of protected messages from one node to another.
Our plan is to use standard protocols SMTP, POP3 and IMAP for
create a universal interfaces between user and other nodes in the BitDust network.

At the begining of the client software, will be started a couple local mail servers for input and 
output mails. This servers is pretty small and acts as
intermediate scripts between the user's email client and program BitDust.

After switching on that functionality in the BitDust software, 
the user will only needs to configure a mail client that is most convenient for him.

At the moment there is not a final decision on the format of e-mailboxes
within the network BitDust. Probably they will be formed based on user's IDURL, for example example
http://p2p-id.ru/veselin.xml will be translated to veselin@p2p-id.ru.



## Monetization through cryptocurrency

To create the most equitable relations between users, we plan to introduce
methods to encourage each other to donate resources of own PC to the network.
Each user should have the ability to make a profit
from donating resources of his device to other users of the software.

We plan to use well-known "Cryptocurrencies" to create an electronic "coins".
Such coins can be used to conduct transactions between users and "pay" for services 
of suppliers, scrubbers, routers, id-servers, etc.
Like the well-known BitCoin, it will be possible to create a free conversion of BitDust 
coins into any material assets, including real money in the end.

This will attract real funds to the netowrk with a corresponding increase of the BitDust society itself.

We need to drive the development of the project and people might want to release finaly some sort of electronic "shares" of the BitDust "foundation", 
which will be fully protected by the same way using Blockchain technology.
Anyone will be able to instantly invest in BitDust development process directly from home and gain profits in the future from the growth of capitalization of the entire project.



## Anonymous logon

At the moment, user identification  in the BitDust system let you hide your personal data 
and uses only short text identifiers.
Not required any authorization, provide your email or phone number.
BitDust contributors do not know any overal or detailed info about the users of the software.

However, the user's IP address at this stage of the project development can not be hidden - it 
is published in his identiy file in open or semi-open form.
We can talk about pseudo-anonymity in the BitDust network.

The implementation of the algorithm of hiding the real IP address of the user will provide:

+ anonymously store and distribute data across the network
+ a completely anonymous correspondence
+ create a personal sites whose owners are almost impossible to calculate



## Decentralized social network

Autonomy of each node in the network BitDust allows you to create a fully distributed
and free user community.
The absence of authorization and central nodes will remove strict censorship and "spying" of users.

However, there must be some rules for the interaction and communication - they can be developed
on the basis of already existing popular social networks.

This can lead for interesting social experiments in the entire human society.


## Distributed WEB-hosting

In our long term plans is to create an environment for the development of fully-protected sites. 
Any such site will have no single entry point and placed on many nodes 
in the BitDust network - they can not be closed by any authority.

User's suppliers can be used to maintain a distributed database for his WEB site. 
All HTTP requests from visitors will fall on a random machine in the set of suppliers.
The owner's machine is not involved in the rendering process and it can
leave the network immediately after the initial setup of the entire environment for such WEB hosting.



## Endless virtual worlds

Modern on-line games allow virtual travel in artificially created 3D space,
prepared in advance by the developers. In most games, all static data that are needed 
to display of the 3D world, requires pre-load on the player's computer and periodically updated 
when adding new locations, quests, etc.

However, there are software packages for generating pseudo-random landscapes
according to set parameters. Can be automatically created and other terrestrial objects.

On the basis of a fully distributed storage BitDust possible to implement such storage of 
pseudo-random locations or entire 3D worlds, so that each location will be absolutely unique.

Moving from one location to another can be done completely transparent to the player and will allow 
to travel around the global space.
During the movement of the character on the global map, will be
dynamically loaded adjacent locations from distributed repositories of other users. 
The whole process will happen automatically - long before the player reach the visible horizont 
of the current location, the next piece of global map will already be loaded on his computer 
and rendering process will be continued without delays.

The more players are in on-line game, the more nodes may be used to accommodate generated data, 
and bigger may be the whole virtual universe.

Most interesting is that locations can be created and maintained not by the creators of the game, 
but the players themselves.
Creating a new location can be entrusted to the player, and the creators of the game will only 
exercise coordination and overall management of the virtual universe.

This makes it easy to create a project of unlimited scope, based on the 3D engine of one of 
the on-line games. The interaction of players will happens not through a single dedicated server, 
but directly to each other in the framework of that piece of global map in which 
they are currently located.



<div class=fbcomments markdown="1">
</div>