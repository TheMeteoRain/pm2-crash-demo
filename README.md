# pm2-crash-demo

Sample repository to show how pm2 gives error when using following process file configuration

`module.exports = {
  apps: [
    {
      script: "npm",
      name: "gStash",
      cwd: "./",
      args: "run-script start"
    }
  ]
}`

git clone https://github.com/TheMeteoRain/pm2-crash-demo
npm install
pm2 start .\ecosystem.config.js
pm2 logs
