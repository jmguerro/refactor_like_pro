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

