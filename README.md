# QuickTio
QuickTips to share with people

1. To server static front end you need a simple HTTP server that serves the file, or chrome will complain. `npm install -g http-server`

   Navigate to the folder and run `http-server` and you will see `localhost:8080` available.

   Alternatively, you can pass `-p` flag to set a port number, this allows you to run multiple front-end on one machine without conflict.

   If you don't want open too many terminal tabs to run stuff or the http-server prompt is too annoying, you can add `&` to the end to the command. `http-server -p 9000 &` and hit ENTER twice. This way you can run multiple http-server in the background.

   If you stay in the same command prompt and the log debug message is to annoying, pass `-s` to silent it.

   What about setting up a quick remote demo server and too lazy to install nginx and configure? Because if you ssh into a EC2 instance, run http-server in the background, when you close the ssh session, terminal it will send SIGTERM to the http-server process and kill it. Use `nohup http-server -p 9000 -s &`.

2. Scalable and Intuitive DevOp work flow
        See [link](http://jeffkreeftmeijer.com/2010/why-arent-you-using-git-flow/)
