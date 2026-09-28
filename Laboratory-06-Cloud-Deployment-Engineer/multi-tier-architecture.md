# Two-Tier Architecture

A Two-Tier Architecture separates an application into two main parts. These parts are the Web/Application Tier and the Database Tier.

## The Web/Application Tier

The Web/Application Tier provides access to the user interface. Accepts HTTP requests from users, sends requests to the database where data is stored.

## The Database Tier

Database Tier - Stores persistent data such as user accounts and other application data. It is responsible for data and answers Web/Application Tier requests.

## Why separate them?

Separate Containers for Web Server and Database makes the system easier to manage and maintain. Each of the containers performs a particular function and a problem with one container does not affect the other container directly.
