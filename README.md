This project documents a Thrift error I'm receiving receiving trying to get Suro up and running.

## Start the Server

    java -cp target/my-app-1-jar-with-dependencies.jar com.netflix.suro.SuroServer -m conf/routingmap.json -s conf/sink.json 

## Start the Client

    java -cp target/my-app-1-jar-with-dependencies.jar com.onetag.ExampleClient "localhost:7101" "async" 3

## Witness the Error

    467219 [Thread-4] ERROR org.apache.thrift.server.TNonblockingServer - Read an invalid frame size of 0. Are you using TFramedTransport on the client side?

Help!
