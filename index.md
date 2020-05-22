## Welcome

### My projects

Because I keep learning new things, I keep trying new things. That means that I have a lot of projects, but I do not finish each one or work it out completely.

#### HGLabor <img src="./resources/icons/hglabor_logo.gif" width="40">
HGLabor is a minecraft server originally only providing the gamemode HG (SoupPVP with Kits). It was founded in 2019 by [NoRisk](https://www.youtube.com/noriskk).
Now you can play on the server and enjoy different gamemodes or just hang out in the lobby.
<br>
My role in the team is to code core systems, gamemodes and to manage the project.
<br>
You can visit [hglabor.de](http://hglabor.de) if you want to find more about the whole server.

##### HGLaborSurvival
Currently, I am working on a serverside minecraft modding project. It adds new items with new textures, aswell as other new functionality to the game. The good thing about this is, that the player does not have to download any content by himself, because the vanilla minecraft client already provides a resourcepack-download functionality.
<br>
You can visit the [project website](https://sites.google.com/view/hglaborsurvival/) if you want to learn more.

##### Other
HGLabor is a network, which means that the server actually constist of several seperate servers. These servers are connected via [BungeeCord](https://www.spigotmc.org/wiki/bungeecord/) (a software provided by the Spigot Team). The seperation brings a lot of advantages, but one disadvantage is, that servers cannot communicate easily anymore. That is why I developed a *ServerCommunicator* which uses Redis and extends it with message callbacks inside of BukkitRunnables in order to efficiently and easily run any functionality when receiving a message.
<br>
Also, the network needs a hub/lobby (*HGLaborLobby*). It solves as a fallback server aswell as hub for players choosing a gamemode to play next. This hub provides other features aswell.

#### Spamgourmet Reloaded
[Spamgourmet](https://spamgourmet.com) is an E-Mail service which purpose it is to save you from companies selling your E-Mail Address to third party spammers. But its future is/was not unclear, which motivated me to recreate this service (again with the purpose of learning new things while creating an online service with both server and client (browser) -side programming). My recreation of the service is currently not online, because I still have to fix a few things before I am sure I can release it.
<br>
Spamgourmet was split into two halfs:
- a Java part receiving and sending the E-Mails
- a Website part constisting of clientside JavaScript and serverside PHP

You can read more about the current state of the original spamgourmet service in this [forum post](https://bbs.spamgourmet.com/viewtopic.php?f=7&t=1793&sid=5a5448445da031e1773bd777b125f903).

#### Olymp
Olymp is a minecraft server I created a lot of years ago. I learned to program with this project, by using Java and the minecraft-server software [spigot](https://spigotmc.org) as a dependecy.
<br>
The server made it possible that I could try new things and learn a lot of new techniques, aswell as managing a player base.

##### OlympSurvival
Olymp survival is a seperate server from the main Olymp server and provides a pure vanilla minecraft multiplayer survival experience. What I coded for this project are features not destroying this experience, but bettering the overall system for multiplayer servers.
<br>
Also, we built a nice survival world on this server 🙂

##### GameTest OpenGL
This project has no real name as it is a learning project only. I wanted to learn OpenGL without the help of any engine, and that is why I decided for [LWJGL](https://www.lwjgl.org/), a game library for java. It provides OpenGl and a lot of other bindings for Java. To learn this rather complicated topic, I followed [this](https://ahbejarano.gitbook.io/lwjglgamedev/) tutorial.
<br>
I extendend the tutorial code here and there, and even worte *my own* `.obj` *file parser*.

#### Processing Pong
// TODO

#### Python in School
// TODO
