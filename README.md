# app-running-another-port
example: Something is already running on port 3000. 

terminal:
? Something is already running on port 3000. Probably:
  /root/.nvm/versions/node/v14.18.2/bin/node /home/workspace/reactjs/coding-practices/destinationSearch/node_modules/.pnpm/react-scripts@4.0.3_react@17.0.1/node_modules/react-scripts/scripts/start.js (pid 17958)
  in /home/workspace/reactjs/coding-practices/destinationSearch

Would you like to run the app on another port instead? › (Y/n)

steps to solve above issue:

lsof -i :3000
kill -9 17958
npm start
