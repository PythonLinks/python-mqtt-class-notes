# python-mqtt-class-notes
These are the instructions for a Python MQTT class.
There are two parts to the class.  First we build a client
application.  Really two applications, one to subscribe and one to publish.
Then we will fire up a server.




## Client Exercises
These exercises are based on the client.py file in this repository. 

1. Connect to the MQTT server.

2. On Connect, go ahead and subscribe.  You can do it right after the connect,
but more interesting to do it on subscribe.

3. OnSubscribed, go ahead and publish a message.  Again you can probably do it
right after the connect/subscribe command, but more interesting to do it onSubscribed
You learn how the call backs work.

4. Okay, and now you can create a similar application for waiting at the terminal and
publishing what you type.  But give it a very very long connection time out. 

## Broker Exercise
I will first lead a discussion of the different brokers.
Basically Mosquitto with the go auth plugin seems to be the richest and most stable.
Hive in Java is interesting. Polished and expensive. 
EMQX in Erlang has lots of functionality.
Emitter.io in GoLang is interesting, but odd. 

1. Now go ahead and fire up a broker.  
https://hub.docker.com/r/pythonlinks/letsencrypt-mosquitto

2. Make sure it works using MQTT Explorer.

3. Connect your client and server to it. 
