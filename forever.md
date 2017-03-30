I like PM2 more now, use [PM2](pm2.md)
###forever
NPM module that watches your node app and re-runs it if it crashes. [forever on npm](https://www.npmjs.com/package/forever)

Installation
```
npm install forever -g
```
Run a node app forever (restarts on crashes, not reboots)
```
forever start /path/to/node/project/app.js
```

Run a node app (started via npm script) forever (restarts on crashes, not reboots)
from inside `/path/to/node/project/`
```
forever start -c "npm run start" ./
```
