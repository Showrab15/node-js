1. How to install node express ?

i. go to node express website

ii. then go to the getting started site

iii. give this command in your prompt code after going projects folder : mkdir folder-name

iv. go that app by : cd folder-name

v. give this command for initialize node express : npm init -your

vi. then install express by this command : npm install express

vii . then give this command : nodemon index.js

viii . then go to the folder which you install node express by using : code .

ix. create a index.js file in your folder

x. create a folder named (data or something), & then create a .json file in this folder for contain your json data 



xi. After pushing these code in your index.js file you must be install cors .

xii. go to the resources site in the express website

xiii. then go midddleware from resources

xiv . then go the cors option

xv. then give this command in your prompy code in that folder which you install node express :  npm install cors

xvi.  then write these code in your index.json file

const express = require('express');
const app = express();
const cors = require('cors')
const port = 5000;

const catagories = require('./data/catagories.json');

app.use(cors())

app.get('/', (req, res) => {
res.send('dragon is running')
})



app.get('/catagories', (req, res)=>{
    res.send(catagories)
})

app.listen(port ,()=>{
    console.log(`dragon api is running on ${port}`)
})




xviii. for every time on server site give this command or press up arrow of the keyboard:  nodemon index.js

