# Typing Indicators with PubNub Signals

Build your chat app typing indicators with PubNub Signals, a PubNub Pub/Sub Messaging API.

## What is PubNub?

PubNub is a globally distributed data stream network. Deliver data between devices with low latency, regardless of location, using the Pub/Sub messaging design pattern. PubNub scales to any user volume or message volume instantly. There are more than 70 SDKs so you can write PubNub code fast, in any language.

## What is PubNub's PubSub Messaging?

Send 32KB or smaller messages to any active subscribers. Publishers can be any device that knows TCP. Published messages are replicated to all PubNub global data centers. Published messages can be stored in History, or invoke a PubNub Function.

## What is a PubNub Signal?

A Signal is the same as a PubNub Publish except it can only be 30 bytes in size or smaller. Signals are not replicated to all global data centers, they can only be delivered to subscribers in a single region. They are not stored in History for a later fetch; only the most recent Signal message can be fetched later. Signals are **cheaper** than Publishes when your app is at scale.

## Why Use Signal Instead of Publish?

PubNub Signals are meant to include the same reliability and latency as PubNub Publishes, but they are for non-critical data stream messaging. I.E. Chat Typing indicators, Live GPS Location Update Stream, Live Sensor Update Streams from IoT devices.

## Typing Indicator Demo

Open the HTML page of a simple chat demo. The chat includes Typing Indicators powered by PubNub Signals. This will save you money when your chat app is at scale. Using PubNub Publishes for Typing indicators can be expensive at scale, Signals are your cheaper alternative for non-critical real-time messaging.

Click Here for the Live JS Chat Demo with Typing Indicators

**Use Incognito for a 2nd unique user ID**

![PubNub JS Chat Typing Indicator Demo](https://i.imgur.com/xsqD5Mi.gif)
