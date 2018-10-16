# Distributed Systems and their Features
## Case Nr. 1
A server program written in one programming language (for example C++) provides the implementation of a BLOB (Binary Large Object) object that is intended to be accessed by clients that may be written in a different language (for example Java). The client and server computers may have different hardware, but all of them are attached to an internet.

###### *Question*
Describe the problems due to each of the five aspects of heterogeneity that need to be solved to make it possible for a client object to invoke a method on the server object.

###### *Answer*
In this case, we will assume that the Internet manages the differences between the networks. We will proceed here to several operations of sending and receiving messages.
As it is said in the question we have the language, C ++ and Java, each has its type of representation of data structures, so it is necessary to create a common link for the entire data structure that will allow sending of the message to the recipient. For that we will first, use a common set of communication protocols.
Then for the heterogeneity of the material, it is necessary to have a standard to represent the elements of data.
But to solve these problems, it is important to share the standards so that the implementers are not different.
Then to have independent standards for the transmission of data structures.

So It is therefore necessary to use a common set of communication protocols. For deal with the heterogeneity of the material, we will make a standard for representing the data elements. But also make a common standard for conveying the message. And an independent standard for representing data structures.


## Case Nr. 2
###### *Let us contunue with a situation from Case Nr. 1*
An open distributed system allows new resource sharing services such as the BLOB object mentioned in Case Nr.1. 
to be added and accessed by a variety of client programs. 
###### *Question*
Discuss in the context of this example, to what extent the needs of openness differ from those of heterogeneity.

###### *Answer*
In this context the standards are different. They must first be pooled before the implementation of the BLOB object. Thus the developers are obliged to agree on the standards.  If we want the clients to access the interface with the BLOB object. It must be published as soon as it is in the system.


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
It may already have problems identifying users. Thus the people allowed to access the information protect and in the messages requests will not work. Then you have to check that the identity of the user is correct and prevent other users from creating problems with the messages.
But there can also be problems when returning information. Thus, messages should be encrypted to prevent message interception.
