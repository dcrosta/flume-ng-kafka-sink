flume-ng-kafka-sink
================

This project is used for [flume-ng](https://github.com/apache/flume) to communicate with [kafka 0.8.0](https://kafka.apache.org/documentation.html#quickstart).

Configuration of Kafka Sink
----------

    agent_log.sinks.kafka.type = org.apache.flume.sink.kafka.KafkaSink
    agent_log.sinks.kafka.channel = all_channel
    agent_log.sinks.kafka.zk.connect = 127.0.0.1:2181
    agent_log.sinks.kafka.topic = all
    agent_log.sinks.kafka.batchsize = 200
    agent_log.sinks.kafka.producer.type = async
    agent_log.sinks.kafka.serializer.class = kafka.serializer.StringEncoder
    # support all properties defined at : [kafka producer configs](https://kafka.apache.org/documentation.html#producerconfigs)
    agent_log.sinks.kafka.request.required.acks = 1

Special Thanks
---------

In fact I'm a newbie in Java. I have learnt a lot from [flumg-ng-rabbitmq](https://github.com/jcustenborder/flume-ng-rabbitmq). Thanks to [Jeremy Custenborder](https://github.com/jcustenborder).

