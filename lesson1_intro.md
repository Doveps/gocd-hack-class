# GoCD and Jenkins
* Diamond dependency
* One sibling fails
* Does it block the stream?

# First look
* open http://localhost:8153/go/pipelines
* pipelines
* compared to jenkins jobs
* click AppDevelopment label: 1
    * click pipelines
* click AppDevelopment first green bar
* click FirstJob
* click Console

# On the command line
## Get a root shell on your VM
```
vagrant ssh
sudo -s
```

## Is the server up yet?
```
cd /var/log/go-server
less go-server.log
/Finished notifying all listeners
```

## Check for agent and server processes
```
ps -efHwww
```

## Run as the go agent
Always debug as the go user!
```
su - go
```

## Look at the agent working directories
```
cd /var/lib/go-agent/pipelines
ls
cd Shared_Services
git remote -v
```

# Build our own!

## First pipeline
* TODO

## Build out the value stream
* TODO
