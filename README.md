# dChat
Simple 1-to-1 secure chat (AES-256 Encryption).

The encryption process is client-side (via CryptoJS), so the server will never know the message's plain text.


### Requirments:
- JavaScript must be enabled in the browser, dChat has no external resources
- The server must has read/write file permission


### Installation:
- clone the project repository OR download the files and extract them on your server, for example in: mysite.com/dchat/
- go to: mysite.com/dchat/dchat.php to start


### How it works:
This script can be used to make simple encrypted chat. The message are encrypted in the client side using a common Secret Hash (IV) before sending it to the server that will use a file based database with the encrypted message.


### security:
The encryption alogarithm used is AES-256 with IV, it is the most secure encryption method ever existed. All messages are encrypted locally, and only the chat parties can see the messages. Of course, for maximum security, you must install this script on a secure server, with SSL/HTTPS support.
