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

source code: 