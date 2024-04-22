# Reflection 1

**How many data your publisher program will send to the message broker in one run?**

In one run, the publisher program will send 5 message to the broker including the data of Amir, Budi, Cica, Dira, and Emir.

**The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?**

It means the publisher program will send the message to the same server where the subscriber program receive. The username and password also has the same value which means that the publisher and subscriber is the same account.

# RabbitMQ Screenshot

![RabbitMQ Overview Screenshot](/assets/rabbitmq-overview.png)

# Terminal Screenshot of Publisher & Subscriber

![Terminal Screenshot](/assets/terminal.png)

The bottom terminal is the docker terminal. The left is publisher and the right is subscriber. From the screenshot, we can see that the subscriber terminal generates the same value which are printed in the publisher when _cargo run_ was run. This shows that the message was succesfully sent with RabbitMQ.
