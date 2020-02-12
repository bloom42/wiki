You can find here all the lessons we learned the hard way...

## Never use Docker with the `--rm` flag in production

it will delete the logs, so if something fail, all the logs are lost.