# Logstash-RabbitMQ
Get data from rabbitmq queues to ELK
Use this filter to pull data from RabbitMQ queues (aliveness-test, ha.messaging-buffer, ha.messaging-buffer-failed and  messaging-buffer-unrecoverable)
and upload it to elasticsearch. This filter uses http_poller and calls the HTTP APIs that rabbit exposes

The script will drop records if the queue is empty.
