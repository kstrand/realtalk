# pull tweets off twitter's streaming API and 
# stuff them into a redis set:
tweet_harvester: bundle exec ruby harvest-tweets.rb

# pull tweets out of redis and serve them up (via server-sent events)
# to the browser every second:
web: bundle exec thin --timeout 0 -p $PORT -R config.ru start
