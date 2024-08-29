```
const {Redis} = require("ioredis")

const redisClient = Redis.createClient();

const init = async() => {
await redisClient.set("user:7","Bhuvaeshwari7");
const val = await redisClient.get("user:7");
if(val){console.log(val)}else{console.log("waste Redis")}
}

init()

```
