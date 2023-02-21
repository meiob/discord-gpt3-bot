
![hero image openAI x Discord x Node.js](https://assets.cdn.prod.twilio.com/images/MBw2s9oFEFXHmGTcKG6kYjj9JixmUwE3.width-1616.format-webp.webp "PATEL")

Ready to create a Discord bot with a side of dark humor and gen z slangs, all powered by the unstoppable GPT-3? Let's go!

First things first, we need to hook up our Discord bot with GPT-3, the artificial intelligence language model that makes us question our own intelligence. It's like the "Big Brain" meme on steroids.

Here's some code to get your Discord bot rolling with Node.js:

```js
const Discord = require('discord.js');
const client = new Discord.Client();
const { Client } = require('openai');

client.once('ready', () => {
  console.log('Sup fam, I\'m ready to spit some AI-powered lines!');
});

client.on('message', message => {
  if (message.content === '!hello') {
    message.channel.send('Hey yo, what\'s good?');
  }
});

client.login('your-secret-bot-token-here');
```

This code initializes a Discord client that's ready to throw some serious shade. We've also set it up to respond with a "Hey yo, what's good?" when a user types "!hello". Nothing like a little greeting from an AI language model to make you feel loved, am I right?

Now, let's see how we can use GPT-3 to generate some spicy responses. Check out this code snippet:

```js
const client = new Client({
  api_key: 'YOUR_SECRET_API_KEY',
});

const prompt = 'Yo, GPT-3, hit me with some dank lines.';
const parameters = {
  prompt,
  temperature: 0.7,
  max_tokens: 50,
};

client.completions.create(parameters)
  .then(response => {
    console.log("GPT-3 said: " + response.choices[0].text);
  })
  .catch(error => {
    console.log("GPT-3 couldn't come up with anything, bruh: " + error);
  });

```
This code sets up a new OpenAI client and generates a response using the 'completions.create' method. You can set different parameters like temperature and max_tokens to get different responses. It's like talking to a really smart friend, only this one's an AI.

### Wrok cited

• [DHRUV PATEL](https://www.twilio.com/blog/author/dhrpatel), Twilio Blog, Build a GPT-3 Discord Chatbot with Node.js (Accessed 2023/02/20) [https://www.twilio.com/blog/build-gpt-3-discord-chatbot-node-js](https://www.twilio.com/blog/build-gpt-3-discord-chatbot-node-js).

README author: ChatGPT, @meiob
