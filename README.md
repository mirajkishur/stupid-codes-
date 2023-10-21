const { Client, GatewayIntentBits } = require('discord.js');

const client = new Client({ intents: [GatewayIntentBits.Guilds, GatewayIntentBits.GuildMessages] });

const token = ''; 

client.on('ready', () => {  console.log(`Logged in as ${client.user.tag}`);});

client.on('messageCreate', (message) => {  if (message.content.toLowerCase() === '/hi ncs') {    message.reply('oh,hello!');  }});

client.login('');
