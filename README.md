const { Client, GatewayIntentBits } = require('discord.js');

const client = new Client({ intents: [GatewayIntentBits.Guilds, GatewayIntentBits.GuildMessages] });

const token = 'MTE2NTI0NjE0ODI3ODIyNzAwNA.GjF2BU.a22VVTpJeSyJTp6A_1jlskX6YzD6c6AW2iVDKo'; 

client.on('ready', () => {  console.log(`Logged in as ${client.user.tag}`);});

client.on('messageCreate', (message) => {  if (message.content.toLowerCase() === '/hi ncs') {    message.reply('oh,hello!');  }});

client.login('MTE2NTI0NjE0ODI3ODIyNzAwNA.GjF2BU.a22VVTpJeSyJTp6A_1jlskX6YzD6c6AW2iVDKo');
