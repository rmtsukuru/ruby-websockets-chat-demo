# FancyChat Demo

A simple chat server based off of Heroku's [Ruby WebSockets Chat Demo](https://github.com/rmtsukuru/ruby-websockets-chat-demo).

## Setup
To install all the dependencies, run:

```
bundle install
```

You may wish to delete the existing Gemfile.lock and start fresh unless you too are developing on MinGW/Windows 7.

The application requires (Redis)[https://redis.io/topics/quickstart] to be installed and running locally on its usual port (6379). If you have it running elsewhere modify the REDISCLOUD_URL variable in `.env` accordingly.

Once you have Redis running, start the server:

```
$ bundle exec puma -p 5000
```

You can now visit <http://localhost:5000> to see the application. If you connect to it from multiple browser tabs/windows, all of them will share the same chat.

