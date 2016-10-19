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



| Tables        | Are           | Cool   |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |
