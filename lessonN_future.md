# pipelines, stages, jobs, tasks?
* in GoCD: pipepline, stage, job, task
* parallel vs serial
* best practice? 
* start simple: one task in one job, in one stage, in one pipeline

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
* click pipeline TODO compare
* all code commits and pipeline changes upstream!
* click pipeline TODO changes
* source commit is highlighted

# click on admin
* more advanced topics
* user permissions
* edit config xml

# Sizing
* memory hungry!
* more pipelines, more agents, more memory!
* jvm does not use more than one cpu
* but source control materials do parallelize
* space: holding your old artifacts

# Tricks
* config.xml is a git repo: push periodically!
