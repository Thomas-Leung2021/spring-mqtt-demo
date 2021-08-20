# Spring MQTT Demo
## Run the project
1. Run the Mosquitto MQTT broker in mqttBroker folder: 
```/usr/local/sbin/mosquitto -v -c mosquitto-spring.conf```
2. Run Spring application
3. Open postman, create a POST requiest at ```localhost:8080/sendMessage```

Inside the json body:
```
{
    "topic": "myTopic",
    "message" :{
        "data": "hello world"
    }
}
```
4. After you make the request, you should see the json message in the Spring console

[Reference](https://www.youtube.com/watch?v=HHKrKwI--Yw)