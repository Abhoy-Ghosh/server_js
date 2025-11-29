🌐 Simple Node.js Static File Server

This is a lightweight Node.js HTTP server that serves static HTML pages (index.html, about.html, contact.html) without using Express or any external packages.

The server uses only core Node modules:

http — to create the server

fs — to read files

path — to safely resolve file paths

You can run this project locally to understand how static hosting works internally.

📁 Project Structure
project-folder/
│
├── index.html       # Home page
├── about.html       # About page
├── contact.html     # Contact page
├── server.js        # Node.js server
└── README.md

🧠 How It Works

Whenever someone opens a URL like:

/

/about.html

/contact.html

your server:

Detects the route

Resolves the correct file path

Loads the file using fs.readFile

Determines MIME type (text/html, etc.)

Sends the file back to the browser

🗂 Example Pages
index.html (Home)

Shows: welcome page!!!!!!!!


index

about.html

Shows: about page!!!!!!!!


about

contact.html

Shows: contact page!!!!!!!!


contact

🚀 Running the Server
1️⃣ Install Node.js

Required: Node.js v12+

2️⃣ Start the server
node server.js

3️⃣ Visit in browser
http://localhost:3000

🧩 Core Server Logic (from your server.js)

Your server:

Resolves path safely

Detects extension (.html, .css, .js, .png)

Maps it to MIME type

Sends back the correct file

Handles 404 errors gracefully

Example flow:

Request → Resolve file → Check MIME → Read file → Return response


Server file reference:


explaination

🛠 Features

✔ Serve static HTML pages

✔ No external libraries

✔ Auto-detect file type

✔ Clean MIME type mapping

✔ Proper 404 handling

✔ Terminal logs requested paths

🔮 Possible Improvements

 Add Express.js version

 Add routing system

 Add CSS + JS example files

 Add API endpoints

 Add template engine (EJS / Handlebars)

 Add logs + middleware system

👨‍💻 Author

Abhoy Ghosh
Built using pure Node.js.
