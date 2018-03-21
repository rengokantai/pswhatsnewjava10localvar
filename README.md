# pswhatsnewjava10localvar

## 2. Java 10 Introduction
### 4 Deprecations and Removals
```
javac -h
```


## 3. Local-variable Type Interface
### 1 Introduction bo var
this is legal: var is not new keyword
```
var var="var";
```

### 2 Type Inference
Does this make Java a dynamic language? NO  

Examples:
```
List<String> myList = Collections.<String>emptyList(); //same as
List<String> myList = Collections.emptyList();
Predicate<String> p = (String s)->s.length()>3;
var p = s->s.length()>3;
```

### 3 Demo: Using Var
```
int nums = {1,2,3}; //legal
var nums = {1,2,3} //illegal
```

## 4. Performance Improvements
### 1 G1GC, Parallel Full Garbage Collection
Java9: serial full GC
Java 10: parallel gull GC


### 3 Improved Container Awareness
```
-XX:ActiveProcessorCount=<n>
-XX:InitialRAMPercentage
-XX:MaxRAMPercentage
-XX:MinRAMPercentage
```


