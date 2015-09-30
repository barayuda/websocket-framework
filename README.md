Websocket Framework v0.0.4
======================================

<img src="https://raw.github.com/wmcmurray/websocket-framework/master/screenshots/server.gif" width="300" align="right" title="Server cmd prompt">
This project provide a way to easily create PHP websocket servers and JavaScript clients.
You won't have to deal with socket listening, handshaking, data unmasking and such, it's all done by the framework.

**All you have to do is : create what you have in mind !**

**Licence :** GNU General Public License, version 3.0 (GPLv3)


Features
-------------------------
* Supports **RFC 6455**
* **Easy** to use API
* **Only 10 lines of code** to make a working server
* **Remote control** of servers via a JavaScript client (kick clients, shutdown/reboot server, etc.)
* **Multiple servers** architecture based on the same core
* **A groups system** enabling internal communications between group clients (like a chatrooms in a chat)
* **Connected clients limit** to prevent your servers from exploding


Should you use it or not ?
-------------------------
I won't recommends you to use it for big projects or for production environnement since it's pretty young at this stage. You may want to chose other frameworks with more features. Also, I must admit that the server side language I've chosen (PHP) may not be the best in this context (no multithreading by default, blocking, etc..). You should maybe take a look at Node.js based servers. Despite all of this, I really love to use this framework and I'll be pushing it further until I reach some kind of positive or negative end.


Documentation
-------------------------
* [How to use : general](https://github.com/wmcmurray/websocket-framework/wiki/How-to-use)
* [How to use : remote admin](https://github.com/wmcmurray/websocket-framework/wiki/Remote-admin)
* [API reference : server](https://github.com/wmcmurray/websocket-framework/wiki/API-reference-:-server)
* [API reference : client](https://github.com/wmcmurray/websocket-framework/wiki/API-reference-:-client)


Demos included
-------------------------
<table>
	<tr>
		<th>
			<h3>Realtime 2D RPG</h3>
		</th>
	</tr>
	<tr>
		<td>
			
			<img src="https://raw.github.com/wmcmurray/websocket-framework/dev/screenshots/demo-game-rpg.jpg" width="694">
			<ul>
				<li>Players state are kept on the server, only keyboard events data are sent</li>
				<li>Client-side movements predictions</li>
				<li>Simple in-game chat</li>
				<li>NPCs with a very basic AI</li>
				<li>Support for different areas with different players inside</li>
				<li>Players state can be saved in text files (JSON format)</li>
			</ul>
		</td>
	</tr>
</table>

<table>
	<tr>
		<th>Realtime Chat</th>
		<th>Remote admin control panel</th>
		<th>Hello world</th>
	</tr>
	<tr>
		<td>
			<img src="https://raw.github.com/wmcmurray/websocket-framework/master/screenshots/demo-chat.gif" width="213">
		</td>
		<td>
			<img src="https://raw.github.com/wmcmurray/websocket-framework/master/screenshots/demo-admin.gif" width="213">
		</td>
		<td>
			<img src="https://raw.github.com/wmcmurray/websocket-framework/master/screenshots/demo-helloworld.gif" width="213">
		</td>
	</tr>
</table>

TODOs list
-------------------------
- [x] Add a raw transport layer (raw_send()) for people who wants full control over optimisation
- [x] Add possibility to create custom admin commands
- [x] Add an helper to save and retrieve data in text files
- [/] Create a 2D game demo <strong>(in progress...)</strong>
- [ ] Create a realtime website demo
- [ ] Create an online radio demo
- [ ] Add an admin command to buffer server errors and retrieve them via remote client
- [ ] Add a way to ban a client definitively with the Admin API

