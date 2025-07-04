# Githu actions 

Githu actions are defined in an Yml file located on the workflows/nameoftheyamalfile.yml

#### Synstax is as follows: 

### "name" is where we need to define name of the action
```
name: name of the action
```

### "on" is where we need to define events when the actions should work. 
Events that trigger workflows https://docs.github.com/en/actions/reference/events-that-trigger-workflows <br>

```
on :  
  push:
   brances: [ master] 
  pull+request:
   brances: [ master]
```

### "jobs" are a group of actions that will execute 

```
jobs: 
  build:
  runs-on: ubuntu-latest
    steps: 
    uses: actions/checkout@v4
    
    -name: hello world
    run: echo Hello world!

    -name: pwd
    run: pwd


```
