# Read.Me


## Solution 

1. Initiate a max value variable 

```
    let maxVal = 0; 
```

2. If the weights are equal, add both to max value. 
    
    if(weight1 + weight2 <= maxW){
        maxVal = value1 + value2
    } 
 ```
 
 3. If not, check for every other combonination. 
 
 ```
    
    else {
        if(weight1 <= maxW && value1 > value2){
            maxVal = value1
        } else if (weight2 <= maxW && value2 > value1) {
            maxVal = value2
        } else if (weight1 > maxW && weight2 <= maxW){
            maxVal = value2
        } else if (weight2 > maxW && weight1 <= maxW){
            maxVal = value1
        } else if (value1 === value2 ){
            maxVal = value1
        }
    }
  ```
  
  4. Return max value.
  
  ```
    return maxVal
```
