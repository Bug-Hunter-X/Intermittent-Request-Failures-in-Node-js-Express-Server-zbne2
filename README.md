# Intermittent Request Failures in Node.js Express Server

This repository demonstrates a common issue in Node.js Express servers where requests intermittently fail to receive a response, particularly under stress. The problem stems from improper handling of asynchronous operations and potential resource exhaustion.

## Bug Description

A simple Express server is designed to respond with "Hello World!" after a 5-second delay.  Under normal conditions it works correctly. However, when subjected to a high volume of concurrent requests, the server may fail to respond to some of them. This is due to the server becoming overloaded, unable to process the incoming requests.