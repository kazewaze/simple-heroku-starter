![Logo](/assets/logo.png)

## A simple express.js starter for heroku.

A bare bones starter for someone wanting to build an express app hosted on heroku.

Before beginning make sure you complete these requirements:
- [Create a free heroku account](https://signup.heroku.com)
- [Install the heroku cli](https://devcenter.heroku.com/articles/heroku-cli)
- [Install git and set it up](https://git-scm.com/downloads)
- [Install node.js](https://nodejs.org)

To get rolling with this simple starter just follow these steps:
1. Clone repo or download zip file.
2. Open Command line and navigate to the root directory (ex: $ ```cd simple-heroku-starter```).
3. Enter```git init && git add . && git commit -m "first commit``` into command line.
4. Enter ```heroku login``` into command line and login to your heroku account.
5. Once logged in enter ```heroku create``` or for a desired app name -->```heroku create <your-app-name>```.
6. Now enter ```git push heroku main``` and your app will be live shortly! Now edit the code and get to building your app!
7. Have Fun!

The index.js file is shown below:

```js
// The code is bare bones intentionally.

const express = require('express');

const app = express();
const port = process.env.PORT || 3000;

app.get('/', (req, res) => {
  res.send('Hello world!');
});

app.listen(port, () => {
  console.log(`Listening on port ${port}`);
});
```

Cheers, Kaycee Ingram