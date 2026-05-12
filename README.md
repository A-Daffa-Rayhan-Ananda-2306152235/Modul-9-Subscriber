## Reflection

### a. What is AMQP?

**AMQP** stands for **Advanced Message Queuing Protocol**. It is an open standard, application-layer protocol used for message-oriented middleware.

In simpler terms, it's the standardized set of rules that programs use to securely and reliably send messages back and forth through a message broker like RabbitMQ. It dictates how messages are queued, routed, and delivered between your publisher and subscriber applications.

### b. What does `guest:guest@localhost:5672` mean?

This string is a connection URL used to connect your application to the RabbitMQ server. It follows a standard format: `username:password@hostname:port`.

Here is the exact breakdown of each part:

* **The first `guest`:** This is the **username**. By default, RabbitMQ creates an administrative user named "guest".
* **The second `guest`:** This is the **password**. By default, the password for the "guest" user is also "guest".
* **`localhost:5672`:** This specifies **where** the message broker is running.
    * `localhost` means the broker is running on your local machine.
    * `5672` is the standard default **port number** that RabbitMQ uses to listen for incoming AMQP connections.