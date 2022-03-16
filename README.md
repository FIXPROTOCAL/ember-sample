# SAMPLE OVERVIEW

This project demonstrates how to use Deltix Execution Server (Ember) Java API to send orders and reliably track order state.

> CAUTION: This sample uses TCP-based API to communicate with Ember. Communicating with UDP/IPC based Ember API gateway will be slightly different.


# SAMPLE INDEX

This project includes the following samples:

* DuplexSample - illustrates how to send trading requests and receive events.
* PublicationSample - illustrates how to implement one-way flow of trading requests from client to Ember.
* SubscriptionSample - illustrates how to implement one-way flow of trading events from Ember to client.


# BUILD

To build the project edit `gradle.properties` and correct location and version of Ember installation (or repository):

```
emberdir=D:/projects/deltix/ember
emberVersion=1.7.19-SNAPSHOT
```

Then run Gradle build:

```
./gradlew clean build 
```

# RUN

Make sure Ember is running. This sample assumes it is running locally on port 8989.

The following command line launches DuplexSample:

```
./gradlew run
```