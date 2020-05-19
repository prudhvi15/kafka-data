# kafka commands used by prudhvi
Every command is runned in a seperate window.
1. ```.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties``` is used to run zookeeper service.
1. ```.\bin\windows\kafka-server-start.bat .\config\server.properties``` is used to run kafka service.
1. ```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic gameofthrones``` is used to create topic.
1. ```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list``` is used to display the list of topics.
1. ```.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic gameofthrones``` is used to run kafka producer. This will provide a prompt to enter messages.
1. ```.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic gameofthrones --from-beginning``` is used to run kafka consumer and to show messages from the beginning.
