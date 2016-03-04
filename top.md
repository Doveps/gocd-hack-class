# Before you start
* Install VirtualBox https://www.virtualbox.org/wiki/Downloads
* Install Vagrant https://www.vagrantup.com/docs/installation/
* Download and start GoCD VM https://www.go.cd/2015/08/05/Go-Sample-Virtualbox.html
* Be able to SSH to the VM: vagrant ssh
* Have basic Ubuntu command line familiarity
* Have a Github account https://github.com/join
* Have basic git command familiarity https://guides.github.com/activities/hello-world/
* Fork sample repo: TODO
* Clone this training repo: TODO

# First look
* open http://localhost:8153/go/pipelines
* what are we looking at?
* pipelines, compared to jenkins jobs
* in GoCD: pipepline, stage, job, task
* why the division?
* parallel vs serial
* best practice? start simple: one task in one job, in one stage, in one pipeline

# click on agents
* we start with one
* like jenkins slaves
* server sees new material, asks to execute with material
* agents poll server, pick up jobs
* unit of execution is the job, not the stage

# click on environments
* ties pipelines to agents
* start simple: one environment, one agent
* later, multiple environments
* pipelines choose one environment
* agents choose multiple environments

# click on pipeline TODO, label TODO (NOTE: find one at end of stream)
* value stream
* implications
* invisible blockers
* be ready culturally
* everything is linked together
* fix blockers before adding more features

# click on pipeline TODO play button
* what does yellow mean?
* click on yellow
* click on console button
* what agent is it running on?

# vagrant ssh
* cd TODO
* echo junk >> TODO
* git add -A
* git commit -m test
* what happens on pipelines?
* click pipeline TODO compare
* all code commits and pipeline changes upstream!
* click pipeline TODO changes
* source commit is highlighted

# click on admin
* more advanced topics
* user permissions
* edit config xml

# Build our own!
* Let's add your repo to the stream
* TODO

# Sizing
* memory hungry!
* more pipelines, more agents, more memory!
* jvm does not use more than one cpu
* but source control materials do parallelize
* space: holding your old artifacts

# Tricks
* config.xml is a git repo: push periodically!
