# discord-bots-api
You can report about the api!

# Npm Package
- https://www.npmjs.com/package/discord.dbl

# #FAQ
- Where to get API token
> You will get the api token in your bots edit page!

# Stats Posting


```js
const dbots = require("discord.dbl");
const dbl = new dbots("API-TOKEN-HERE", client);

client.on("ready", async () => {
  dbl.postStats(); => Note: You can only use this package for discord.js use
  // console.log("Server count posted")
  })

//Able to post both server & shards count.....
```

# Has Voted 

```js
const dbots = require("discord.dbl");
const dbl = new dbots("API-TOKEN-HERE", client);

client.on("ready", async () => {
  
let hasVote = await dbl.hasVoted("BOT-ID");
  if(hasVote === true) {
    console.log("Voted")
  } else {
    console.log("Vote please.")
  }
  
});
```

# Search For Bots

```js
const dbots = require("discord.dbl");
const dbl = new dbots("API-TOKEN-HERE", client);

client.on("ready", async () => {
  
  let search = await dbl.search("BOT-ID")
  console.log(search)
  
});
```


