# pm2 

> ### Installation

    $ npm install pm2@latest -g

> ### Usage

    $ pm2 start app.js
    
> ### Application declaration
  #### process.yml

    apps:
    - script   : app.js
    instances: 4
    exec_mode: cluster
    - script : worker.js
    watch  : true
    env    :
    NODE_ENV: development
    env_production:
    NODE_ENV: production   

    $ pm2 start process.yml
    
> ### 文件夹结构

+ $HOME/.pm2 包含所有 pm2 最新文件
+ $HOME/.pm2/logs 包含所有应用日志
+ $HOME/.pm2/pids 包含所有应用 pids
+ $HOME/.pm2/pm2.log PM2日志
+ $HOME/.pm2/pm2.pid PM2 pid
+ $HOME/.pm2/rpc.sock Socket file for remote commands
+ $HOME/.pm2/pub.sock Socket file for publishable events
+ $HOME/.pm2/conf.js PM2 Configuration



| Tables        | Are           | Cool   |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |
