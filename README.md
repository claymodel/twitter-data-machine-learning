twitter-data-machine-learning
====================

## Crawl tweets
* Download Tweets: 
```mvn clean compile  exec:java -X -Dexec.mainClass="jp.elias.tweets.TweetCrawler"```
* ```cd twitter-data-machine-learning```
* ```Run mvn clean package```
* ```chmod 755 target/appassembler/bin/app```

## Training the system
* ```target/appassembler/bin/app -mode train -appKey <appKey> -dataFile <Full or relative path>``` 

## Test

* ```target/appassembler/bin/app -mode recommend -appKey <appKey> -engineName <engine name> -uid <The twitter user id (unsigned integer)>```
