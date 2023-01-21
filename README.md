# kafka

# Confluent Kafka Setup on mac.

## Prequisites

1. Dowload java from https://www.java.com/en/download/.

2. Install by clicking on java dmg file.

3. After installation, verify by entering cmd 'java -version' in terminal.

## Download and configure confluent kafka for local development

1. Goto https://www.confluent.io/get-started/?product=software. 2. Fill the form with full name, email address and select country.

3. Click on start free button.

4. Download TAR version of confluent under Local section.

5. This will download confluent kafka platform 6. Extract downloaded tar file into desired folder.

7. Open server.properties file from /Your/Path/confluent-7.2.2/etc/kafka in desired

8. Uncomment 'listeners' property. Change from listeners=PLAINTEXT://:9092 to 9. Uncomment 'advertised.listeners' property. Change from advertised.listeners=

advertised.listeners=PLAINTEXT://localhost:9092.

10. Uncomment 'listener.security.protocol.map' property.

## Configuring confluent startup in .zshrc

1. Open terminal..

2. Goto root path by commad 'cd -' and enter.

3. Type cmd 'nano .zshrc' and enter.

4. Add below env variables in .zshrc editor.

5. Click on ctrl+X to exit and save.

6. Set.zshrc as source by cmd 'source.zshrc'.

export CONFLUENT HOME=/Your/Path/confluent-7.2.2

export PATH=$PATH:SCONFLUENT_HOME/bin


Run -> confluent local services start

confluent local start

https://docs.confluent.io/5.5.0/quickstart/ce-quickstart.html

confluent local destroy


