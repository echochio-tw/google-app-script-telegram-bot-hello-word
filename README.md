# google app script telegram bot hello word

```
function main() {
  var botSecret = "610418XX:AAGBzrJ5dYipW0xxxxxxxxxxxxx";
  var body = "Hello world !";
  var chatId ="-351xxx";
  sendTelegramNotification(botSecret, chatId, body);
}

function sendTelegramNotification(botSecret, chatId, body) {
var response = UrlFetchApp.fetch("https://api.telegram.org/bot" + botSecret + "/sendMessage?text=" + encodeURIComponent(body) + "&chat_id=" + chatId + "&parse_mode=HTML");
}
```
