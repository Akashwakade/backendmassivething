# backendmassivething

steps for deploying on vercel
create backend repo
npm i json server 
 npm init -y 
create folder index.js and db.json copy db data
then go to cyclic for the creating link for backend select backend repo you will get link
you will get backend data link copy paste it to require places
 copy boiler code paste to index.js
3)const jsonServer = require('json-server')
const server = jsonServer.create()
const router = jsonServer.router('db.json')
const middlewares = jsonServer.defaults()
const PORT = process.env.PORT || 8000

server.use(middlewares)
server.use(router)
server.listen(PORT, () => {
  console.log('JSON Server is running')
})


inside project
5)vercel
6) everything yes except modify changes and existing project

