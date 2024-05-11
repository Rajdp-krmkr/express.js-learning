# How to create a simple & basic express server: 
1. Create a folder.

2. open this folder in terminal (May be in vs code or system terminal).

3. For creating a express project , type in terminal 
`npm init -y`.

4. Type `npm i express` for installing express in that project.

5. create a file (e.g `server.js`) and type the code below:

```const express = require('express')
const app = express()
const port = 3000

app.get('/', (req, res) => {
  res.send('Hello World!')
})

app.listen(port, () => {
  console.log(`Example app listening on port http://localhost:${port}`)
})
```
6. Now in terminal , open the previously made folder and type `node server.js`.

7. To avoid the frequently refreshing problem , use nodemon. Type :
`npm i nodemon` and restart the `server.js` file by typing : `nodemon server.js`.
