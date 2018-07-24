# js-chatlab
notes from lighthouselabs

Enhancements As Challenges 💪

Want to take your code a little further? You may have noticed some bugs and broken features with this app. Try figuring out these fixes on your own - remember, Google is a Developer's best friend.

Initial field - Part I
The initials input field (the first input box) is not being used at all. Modify the app.js so that it sends (emits) the text as something like "DV says: hello" where "DV" is from the first input field (with id="initials") and "hello" is from the message field.

Initial field - Part II
The initials input field is actually meant to be 2 letter initials only. Make it so only a maximum of two characters can be entered into that field.

Hint: Google "html input field maximum length" for a convenient HTML attribute that can be added to your HTML file.

List of Messages
It would be nice to see the message history on the server anytime you join the chat room. Unfortunately, we don't keep/store a message history on the server at all.

One way to do this is to create an empty array that stores the messages.

Then, whenever a message is received on the server, it can push (append) that message string into the array.

Then whenever a user (new socket) connects to the server, (on connection) the server could iterate over all the messages in the array and emit them to that new client/socket.

reference: https://lighthouselabs.ca/ JavaScript Essentials Build a web-based chat app using JavaScript. | Curriculum created by David VanDusen
