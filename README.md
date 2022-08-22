# cindy-kafka-avro-producer-consumer

This project follows this tutorial:
https://medium.com/@affanhasan88/how-to-publish-and-consume-avro-encoded-apache-kafka-messages-using-java-44ed42890637

Background:
-Docker app must be running

1. Add the kafka-clients, kafka-avro-serializer, and Jackson dependency in the pom.xml.
2. Go to https://mvnrepository.com/artifact/io.confluent/kafka-avro-serializer/3.1.1 , click the blue mouse highlighted area(jar 24KB) for download
![Screen Shot 2022-08-22 at 1 44 06 PM](https://user-images.githubusercontent.com/102390736/185995576-52ac87e4-99a6-4b69-8696-2477caf5d060.png)


3. To import kafka-avro-serializer3.1.1 jar, go to IntelliJ > File > Project Structure > Modules > Dependencies > + > JARs or Directories > Select the download > Apply > OK
4. Code the producer class.
5. Code the Customer class.
6. Code the CustomerGenerator class.
7. Code the consumer class.
8. Run the producer class, terminal will look like this:
Published message for customer: <br/> [ Name: customer89 | Email Address: customer89@virtualcompany.com | Phone: +92 0333 325179customer89 ]
9. Run the consumer class, terminal will look like this: 
Message Key:[ customer ] Message Payload: <br/> [ {"contactNumber": "+92 0333 325179customer37", "email": "customer37@virtualcompany.com", "name": "customer37"} ]
10. The producer class terminal will show the serialized message, and the consumer class terminal will show the deserialized message.
