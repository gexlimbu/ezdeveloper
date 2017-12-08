# 3. Auto-follow people who follow a particular Twitter account

There are basically two methods here.

### 1. Follow all the followers of a users:

You can use **copyFollowers** method to follow **ALL** the followers of a given twitter account.
It takes two parameters

* BOT - The bot
* Target - The twitter username (screen name) whose followers the bot needs to follow

#### Syntax
```js
// Now the bot will follow all the followers of user - 'donaldtrump'
copyFollowers(Bot, 'donaldtrump');
```

### 2. Follow only the latest followers of a user:

You can use **getLimitedFollowers** method to follow the latest followers of a user. 
It is, however, limited to 5000 new followers. This method takes 3 parameters

* BOT
* Targett
* Limit

#### Syntax
```js
// To follow the latest 200 users who followed donaldtrump
getLimitedFollowers(Bot, 'donaldtrump', 200)

```

# 4. Follow users who retweet tweets from certain accounts

You can use **trackUsers** method to follow users who retweet tweets of certain USER.
Unfortunately you cannot provide twitter name in this method because that's how twitter API works.
You need to instead provide tweeter ID number which you can get from websites like  

**[http://mytwitterid.com](http://mytwitterid.com/)**

#### Syntax
```js
trackUsers(Bot, '923937847929383928');
```