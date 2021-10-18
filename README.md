#  Super Nimbus Test Project
David Brennan
18/10/2021

## 💬 What is this?
This project is a 2-4 player online game built in the Unity game engine, using the [Nakama Open Source Game Server](https://heroiclabs.com/nakama-opensource/) as a service with Unity.

It demonstrates the following features:
- [Email Authentication](https://heroiclabs.com/docs/authentication/#email)
- [Matchmaking](https://heroiclabs.com/docs/gameplay-matchmaker/)
- C# Dedicated Server Backend (Deprecated to Unity)
- Unity Dedicated Server Backend
- Server Authoritative Movement
- Server Authoritative Collisions
- User Chat
- Player Collectables

## 🛠️ Getting started
# Testing the Game with a Live Server
Before we move further, check that you have the server details quick to hand. We will use this to connect two running game client instances from any machine.

- Download the latest release found in the [releases](https://github.com/daithyy/daithibrennan-supernimbus/releases) section.

- Once you have downloaded the **.zip**, extract the contents under any location. We will only be testing with the Unity **windows_build_game** that serves as the game client.

- Inside **windows_build_game** folder, [allow the TestProject.exe Unity game through your firewall](https://pureinfotech.com/allow-apps-firewall-windows-10/).

- Run two instances of the **TestProject.exe** game.

- Carry out the following steps for both game clients: 

1. Under **Unity Game Server** and **Nakama**, add correct public server IP address found in my email. The ports should remain the same.

2. Under **Login**, input user credentials. A display name, valid email with **@.com** and **ensure your password is longer than 8 characters!**

Example User:

```
Name: Daithy
Email: test@daithy.com
Password: test12345
```

> Ensure the user email is different for both game clients or this will cause an error!

3. Click **Register** for both clients, if you have received a success message; you have registered with the Nakama server.

4. Click **Connect** for both clients, this will start the Nakama matchmaking and will find a match for both players.

5. You should see a successful Nakama validation message in the chat on connection to the Unity game server.

## 🕹️ Controls

- **W** or **Up Arrow** - Move Up
- **A** or **Left Arrow** - Move Left
- **S** or **Down Arrow** - Move Down
- **D** or **Right Arrow** - Move Right
- **Left Shift** - Walk
- **Space** - Jump
- **Y** - Chat

## 📁 Source Code
This repo uses git submodules.

You can clone the project down with `git clone --recurse-submodules https://github.com/daithyy/daithibrennan-supernimbus.git`, to bring all submodules down at once recursively.

## 📥 Release Mirror
- [Download](https://www.mediafire.com/file/p93chs7kfn3b0yy/DAITHIBRENNAN_HIREPROJECT.zip/file)
