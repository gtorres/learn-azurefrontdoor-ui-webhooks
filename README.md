# learn-azurefrontdoor-ui-webhooks

Github webhooks for the azurefrontdoor-ui repo

You'll need bundler

```
gem install bundler
```

The gemfile should take care of the other dependencies.

It's best to set a local bundle path so you won't have to worry about permissions:

```
bundle config set --local path '.gems'
```

Once you run install, you should have all the files you need


```
bundle install
```

One of those files will be Gemfile.lock, which the docker container assumes you have.

Speaking of docker:

build
```
docker build -t <your-tag> . # Make sure you're in the same directory as the Dockerfile
```

```
docker run -p 4567:4567 <your-tag>
```

There is a lot more to know about managing Docker containers, but this will get you started. Docker's website has tons of info to go further.
