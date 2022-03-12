# dbotsonline
# NPM Package
<a href="https://dbots.online/dc" target="_blank"><img src="https://logos-world.net/wp-content/uploads/2020/12/Discord-Logo.png?size=512" alt="Join our discord" width="256"></a><br>
**Support:** [https://dbots.online/dc](https://dbots.online/dc) <br>
**NPM:** [npmjs.com/package/dbots.online](https://www.npmjs.com/package/dbots.online)<br>

<a href="https://www.npmjs.com/package/dbots.online/"><img src="https://img.shields.io/npm/v/dbots.online?style=plastic?maxAge=3600" alt="NPM version" /></a>
<a href="https://www.npmjs.com/package/dbots.online"><img src="https://img.shields.io/npm/dt/dbots.online.svg?maxAge=3600" alt="NPM downloads" /></a>


<a href="https://nodei.co/npm/dbots.online"><img src="https://nodei.co/npm/dbots.online.png?downloads=true&stars=true" alt="npm installnfo" /></a>

## Installation
*If you have trouble with the installation, please feel free to visit our [discord](https://dbots.online/dc) address.*
- `npm i dbots.online`

# Define Module & Client
```js
const Discord = require("discord.js");
const client = new Discord.Client();
const dbots = require("dbots.online");
const dbl = new dbots("TOKEN-HERE", client);

client.login("BotToken");
```

# Server Count & Shard Count Posting
```js
client.on("ready", async () => {
  dbl.serverCount();
  /* 
  -> Server count posted. 
  or 
  -> Server count & shard count posted.
  */

});
```

# Vote Checking
```js
let hasVote = await dbl.hasVoted("671390595184459782"); // -> User ID
  if(hasVote === true) {
      console.log("Voted")
    } else {
      console.log("Vote please.")
  }
// -> Vote please.
```

# Search on dbots.online
```js
let botFind = await dbl.search("842752825888342056");
console.log(botFind.username) // -> Allegro
```
# Python Package
<a href="https://dbots.online/dc" target="_blank"><img src="https://logos-world.net/wp-content/uploads/2020/12/Discord-Logo.png?size=512" alt="Join our discord" width="256"></a><br>
**Support:** [https://dbots.online/dc](https://dbots.online/dc) <br>
**Package:** [pypi.org/project/dbots.py/](https://pypi.org/project/dbots.py/)<br>

<a href="https://pypi.org/project/dbots.py/"><img src="https://img.shields.io/pypi/v/dbots.py.svg?maxAge=3600" alt="PIP version" /></a>
<a href="https://pypi.org/project/dbots.py/"><img src="https://img.shields.io/pypi/dm/dbots.py.svg?maxAge=3600" alt="PIP downloads" /></a>

# Installation
*If you have trouble with the installation, please feel free to visit our [discord](https://dbots.online/dc) address.*
- `pip install bhbotlist`

# Import packages and define client
```py
from dbots.py import dbots
from discord.ext import commands

client = commands.Bot(command_prefix="!") 
dbl = dbots(client,"token of dbots")
```
# Post server count
```py
@client.event
async def on_ready():
  await dbl.serverCountPost()
  print("Posted")

client.run("token") 
```

# Questions?
Come talk to us here:

[![Dbots.online](https://discord.com/api/guilds/950336711752298526/embed.png?style=banner1)](https://discord.gg/xtx49HtRMb)

