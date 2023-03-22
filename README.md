# refactor_like_pro 


### Loop refactor
Loop refactor before :
```java
for(int i= 0; i< items.length,i++){

    // items[i]
}

```

Loop for after refactor :
```java

for (Item item : items){
        // Item
}
```

----------

### Negative conditional refactor
Negative refactor before :
```java
if(!item.name.equals("Aged Brie")){
    if(item.quality > 0){
        ...
    }
}

```

Negative for after refactor :
```java
if(item.name.equals("Aged Brie")){
    ...
}else{
    if(item.quality > 0){
        ...
    }
}
```

----------

### Simple operations refactor
Simple Operations refactor before :
```java
item.quality = item.quality + 1;

```

Split for after refactor :
```java
item.quality +=1;
```
Another refactor for after refactor :
```java
public void qualityIncrement(Item item , int increment){
    item.quality += increment;
}
```


----------

### Extract variable  refactor
Extract variable  refactor before :
```java
item.quality = item.quality + 1;

```

Extract variable after refactor :
```java
if  BOOL_OPERATION_1    
```
Another refactor for after refactor :
```java
Criteria = BOOL_OPERATION_1 + BOOL_OPERATIOB_2;
```


### OOP Pillars

1. Encapsulation
2. Abtraction
3. Polimorfism
4. Inheritance

ideas for Rover Refactor

```java

switch{
    case -> addAxis(1,0)
}

public void addAxis(int addX, int addY){
    return new Point(x + addX,y+addY)
}

switch{
    case -> addAxis(new Point(1,0))
}

public void addAxis(Point point){
    return new Point(x + point.x,y+ point.y)
}
```


Poli example 

```java
Item createItem(name,sellin,amout){
    switch(name){
        case -> "Ham" return new Ham(sellin , amount);
        default ->
    }
}
```


# Agile 

1. Individuals/interactions > Process/tools
2. Working software > comprehensive documentation !!!
3. Customer collaboration > Contract negotation
4. Responding to change > Following a plan
5. Craftmanship > Execution

### Principles of Agile

1. Satisfy the customer early and continuous delivery of valuable software.
2. Welcome changing requirements.
3. Deliver working software frequently from weeks to months , preference short time.
4. Business people and devs working together daily.
5. Build projects around motivated individuals.
6. Face to face conversations to share info.
7. Working software is primary measure of progress.
8. Agile processes promote sustainable development , continuous pace all integrants of project.
9. Continuous attention to technical excellence and good design enhaces agility.
10. Simplicity
11. Self organaizing teams.
12. Team reflect how to be more effective.


        Software Craftsmanship is about professionalism in software development.


