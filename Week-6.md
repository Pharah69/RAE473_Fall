# Distributed Systems and their Features
## Case Nr. 1
A server program written in one programming language (for example C++) provides the implementation of a BLOB (Binary Large Object) object that is intended to be accessed by clients that may be written in a different language (for example Java). The client and server computers may have different hardware, but all of them are attached to an internet.

###### *Question*
Describe the problems due to each of the five aspects of heterogeneity that need to be solved to make it possible for a client object to invoke a method on the server object.
###### *Answer*
Since computers are connected to the Internet, it can be assumed that Internet protocols deal with differences in
networks. But computers may have different hardware, so we have to have to resolve differences in representation of data components of cstomer requests and answer message. computer can run different OS, so we have to make them common; for example, a C++ or Java instruction will be linked by a same operation (depending on the operating system on which it is running).
C++ and Java are different languages using different representation (for example, strings, tables etc...). As I said before, we have to define common standard for each representaion, which would be translated during customer request/answer.





## Case Nr. 2
###### *Let us contunue with a situation from Case Nr. 1*
An open distributed system allows new resource sharing services such as the BLOB object mentioned in Case Nr.1. 
to be added and accessed by a variety of client programs. 

###### *Question*
Discuss in the context of this example, to what extent the needs of openness differ from those of heterogeneity.
###### *Answer* 
To add the BLOB object, requirements from question case Nr.2 must be established; then, standard must be approved and users have to shape with these standards. Furthermore, the BLOB object must allow new and existing user to access to it, and allow different company or workers to work together. 





## Case Nr. 3
###### *We are working with a relevance to situation from Case Nr. 1 about BLOB*
Suppose that the operations of the BLOB object are separated into two categories – public
operations that are available to all users and protected operations that are available only to certain
named users. 
###### *Question*
State all of the problems involved in ensuring that only the named users can use a
protected operation. Supposing that access to a protected operation provides information that
should not be revealed to all users, what further problems arise?
###### *Answer*
To get an access to a protected request, the ID of the user who send the request must be included. This is the cause of several problems like: configure users identity, check if the user identity is right or fake, to avoid user to spam messages, to make protected request secret for other user.
