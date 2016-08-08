
## Sample 1 Hello RabbitMQ

```
    $ node ./1-hello-rabbitmq/receive.js
    $ node ./1-hello-rabbitmq/send.js
```


## Sample 2 Work Queues

```
    $ node ./2-work-queues/new_task.js
    $ node ./2-work-queues/worker.js
```


## Sample 3 publish subscribe

```
    $ node ./3-publish-subscribe/receive_logs.js > ./node_modules/logs_from_rabbit.log
    $ node ./3-publish-subscribe/emit_log.js
```


## Sample 4 routing

```
    $ node ./4-routing/receive_logs_direct.js info warning error
    $ node ./4-routing/emit_log_direct.js error "Run. Run. Or it will explode."
 [x] Sent 'error':'Run. Run. Or it will explode.'
```

## Sample 5 topics

```
   $ node ./5-topics/receive_logs_topic.js "#"
   $ node ./5-topics/receive_logs_topic.js "kern.*"
   $ node ./5-topics/receive_logs_topic.js "*.critical"
   $ node ./5-topics/receive_logs_topic.js "kern.*" "*.critical"
```

## Sample 6 rpc server

```
   $ node ./6-rpc-server/rpc_server.js
   $ node ./6-rpc-server/rpc_client.js 30
```