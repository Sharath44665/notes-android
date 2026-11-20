# Box Layouts

## Using Row

``` kotlin
Row(
            modifier = Modifier.fillMaxSize(),
//            horizontalArrangement = Arrangement.Center
            horizontalArrangement = Arrangement.SpaceEvenly,
            verticalAlignment = Alignment.CenterVertically
        ) {
            Text(text = "a", fontSize = 30.sp)
            Text(text = "b", fontSize = 30.sp)
            Text(text = "c", fontSize = 30.sp)
        }
```

source code: https://gitlab.com/sharath44665/layouts-box-row-column#

## using Column

``` kotlin
Column(
        modifier = Modifier.fillMaxSize(),
//        verticalArrangement = Arrangement.Center,
        verticalArrangement = Arrangement.SpaceEvenly,
        horizontalAlignment = Alignment.CenterHorizontally
    ) {
        Text(text = "Android", fontSize = 25.sp)
        Text(text = "Bird os", fontSize = 25.sp)
        Text(text = "Cache os", fontSize = 25.sp)
    }
```
source code: https://gitlab.com/sharath44665/layouts-box-row-column#