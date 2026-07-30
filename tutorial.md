# My Tutorial

## Step 1
Move the agent onto Plate 1 three times to send an S


```blocks
agent.move(FORWARD, 1)
loops.pause(1000)
agent.move(BACK, 1)
loops.pause(1000)
agent.move(FORWARD, 1)
loops.pause(1000)
agent.move(BACK, 1)
loops.pause(1000)
agent.move(FORWARD, 1)
loops.pause(1000)
agent.move(BACK, 1)
loops.pause(1000)
```


## Step 2
Use a loop to shorten your code
```blocks
for (let i = 0; i < 3; i++) {
    agent.move(FORWARD, 1)
    loops.pause(1000)
    agent.move(BACK, 1)
    loops.pause(1000)
}
```

## Step 3
Turn the agent and step on Plate 2 three times to send an O
```blocks
for (let i = 0; i < 3; i++) {
    agent.move(FORWARD, 1)
    loops.pause(1000)
    agent.move(BACK, 1)
    loops.pause(1000)
}
agent.turn(LEFT)
agent.turn(LEFT)
for (let i = 0; i < 3; i++) {
    agent.move(FORWARD, 1)
    loops.pause(1000)
    agent.move(BACK, 1)
    loops.pause(1000)
}

```

## Step 4
Turn back and step on Plate 1 three times to send the final S
```blocks
for (let i = 0; i < 3; i++) {
    agent.move(FORWARD, 1)
    loops.pause(1000)
    agent.move(BACK, 1)
    loops.pause(1000)
}
agent.turn(LEFT)
agent.turn(LEFT)
for (let i = 0; i < 3; i++) {
    agent.move(FORWARD, 1)
    loops.pause(1000)
    agent.move(BACK, 1)
    loops.pause(1000)
}
agent.turn(LEFT)
agent.turn(LEFT)
for (let i = 0; i < 3; i++) {
    agent.move(FORWARD, 1)
    loops.pause(1000)
    agent.move(BACK, 1)
    loops.pause(1000)
```

## Step 5
Create a function(advanced) so you can reuse the move forward 3 times and turn code


```blocks
function moveForward() {
    for (let i = 0; i < 3; i++) {
        agent.move(FORWARD, 1)
        loops.pause(1000)
        agent.move(BACK, 1)
        loops.pause(1000)
    }
    agent.turn(LEFT)
    agent.turn(LEFT)
}

```

## Step 6
Remember to call your function in your main code
```blocks
function moveForward() {
    for (let i = 0; i < 3; i++) {
        agent.move(FORWARD, 1)
        loops.pause(1000)
        agent.move(BACK, 1)
        loops.pause(1000)
    }
    agent.turn(LEFT)
    agent.turn(LEFT)
}
for (let i = 0; i < 3; i++) {
    moveForward()
}
```







    
