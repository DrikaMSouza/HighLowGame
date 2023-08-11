# Hi-Lo Game

## How to play

After connecting to the URL you can start guessing the mystery number.
Each player gets a random name that can be changed at will.
Any player can guess at any moment. Any player can also change the Game Engine at any time. 

## Overall architecture
The game is built using ASP.Net Core Razor Pages, with SignalR to enable multiplayer.
There is a Game Master responsible for the whole game. 
The Game Master can be configured with an IEngine (Default), but you can implemented more configurations.

## Tests
There is ~90% of code covereage.

## Deviation from C# style guidelines
The naming convention for private and private static differs from the Microsoft's C# style on purpose based on personal preference and industry standards.

## Out of scope
* Have a separate Hub project to support multiple clients.
* Validate the input on the front-end as it is desirable to keep open the possibility of the user type commands as well as guesses.
