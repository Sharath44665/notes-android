# Text Example 

`TextExample.kt` 👇:
``` kotlin
@Preview(showBackground = true, showSystemUi = true)
@Composable
fun TextExample(modifier: Modifier = Modifier) {
    Text(
        text = "Welcome Sharath",
        color = Color.Blue,
        fontSize = 30.sp,
        fontWeight = FontWeight.Bold,
        fontFamily = FontFamily.Serif,
//        letterSpacing = 10.sp
        textAlign = TextAlign.Center
    )
    
}
```

`MainActivity.kt` 👇:

``` kotlin
class MainActivity : ComponentActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        enableEdgeToEdge()
        setContent {
            MaterialTheme {
                Scaffold(modifier = Modifier.fillMaxSize()) { innerPadding ->
//                    Greeting(
//                        name = "Android",
//                        modifier = Modifier.padding(innerPadding)
//                    )
                    TextExample()
                }
            }
        }
    }
}
```

source code: https://gitlab.com/sharath44665/text-example#


