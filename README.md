App with Node.js and Express Basics

1. Install Node.js 
2. Open a command prompt and type: 
   mkdir myappname
   cd myappname
3. Inititalize the project with:
   npm init
4. Once done with the configuration install express
   npm install express --save
5. Start your text editor and create a file named index.js and add:
   var express = require('express');
   var app = express();
   app.get('/', function (req, res) {
   res.send('Hello World!');
   });
   app.listen(3000, function () {
   console.log('Example app listening on port 3000!');
   });
6. Run the app by typing:
   node index.js
7. After running the command, load http://localhost:3000/ in a browser to see the output.
   Your done and ready to start building!!!

   Tips: 
   Use node --watch index.js built-in option to automatically restart the application when a file changes.
   Use node --run test if you have scripts in your package.json. This flag flag allows you to run the specified command