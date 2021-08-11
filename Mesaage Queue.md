# Message Queue

## What is a message queue?

A queue to which messages are sent is called a message queue.
Programs can retrieve those messages, and until they do so,
the messages will remain in the queue.

There is a specific manager called Queue Manager that manages
these queues. The operating system that runs the queue manager
decides the format of the queue.
Programs interacting with the message queue don't have
knowledge about the physical location of the queues.

If programs want to access queues, they can do by the services
provided by the queue manager. Programs can open or close the
queue. They can also send messages to the queue, and retrieve
messages from it.

## Usage

Message queues are generally used for communication among
processes, or among threads of the same process. They can
be used to pass content or control.

The message queue model is similar to the publisher/
subscriber model.

The sender doesn't need to wait for a response from the
receiver. They both don't need to interact at the same time.
This type of communication is called asynchronous communication.

There are limits on the number of messages that can a queue can
hold and the size of the message that is sent.

## Types of Messaging Queues

There are two types of messaging queues

### Point-to-Point

One application can send a message to the queue which can be retrieved by only one application.

In this kind of messaging, the sender needs to know information about the receiver such as the name of the queue and queue manager.

### Publish/Subscribe

In this messaging, there is a publisher which sends the message to all the interested applications. An interested application is called a subscriber. There can be more than one subscriber.

The publisher and subscribers do not need to know information about each other.

## Popular MQ software

* MuleSoft Anypoint Platform
* IBM MQ
* Azure Scheduler
* Apache Kafka
* TIBCO Rendezvous

## Enterprise Service Bus

Enterprise Service Bus or ESB integrates various software
applications. It uses a bus-like infrastructure.
Applications can talk via the bus. For communication, they
do not need to know about other systems on the bus.
In the ideal case, there should be no direct communication between the applications.
ESB is commonly used in a service-oriented architecture (SOA).
ESB is a special kind of client-server model, where any application can behave as a client or server.

The special thing about ESB is that it is platform-independent.
And it can integrate with anything.

Point-to-point integration is hard to manage overtime and
there were other problems as well, which led to the concept of Enterprise Service Bus.

### Benefits of ESB

The main benefits are-

1. It Provides a standard platform for integration
1. Flexibility is increased
1. It provides standard services
1. More configuration instead of integration coding
1. No need for a central regulator


 ## References :

 1. https://www.interlogica.it/en/insight-en/enterprise-service-bus-what-you-need-to-know/
 
 1. https://en.wikipedia.org/wiki/Message_queue#Graphical_user_interfaces
 
 1. https://blog.iron.io/what-is-a-messaging-queue-and-how-can-you-utilise-it/
 
 1. https://en.wikipedia.org/wiki/Enterprise_service_bus
 
 1. https://www.g2.com/categories/message-queue-mq
 
 1. https://www.ibm.com/docs/en/ibm-mq/8.0?topic=overview-introduction-message-queuing
 
