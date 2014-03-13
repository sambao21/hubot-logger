hubot-logger
============

logger.coffee is a script for logging chat activity to Redis.

It provides an HTTP server that allows for
minimalistic log viewing. It also provides some in-chat commands to start,
stop, and pause logging, and to send recent transcripts to users upon request.

This script depends on ```redis```, ```moment```, ```connect```, and ```connect_router```.

*Quick start:* This script works out of the box with no extra configuration (as
long as ```redis-brain``` is set up and working correctly), but it's strongly
recommended that you set ```LOG_HTTP_USER``` and ```LOG_HTTP_PASS``` to change the login
for the logs server from the default, which is

- User: logs
- Password: changeme
