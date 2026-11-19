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


# textfiled:

``` kotlin
@Composable
fun TextFieldExample(modifier: Modifier = Modifier) {
    var name by remember { mutableStateOf("") }
    var passwd by remember { mutableStateOf("") }
    TextField(
        value = name,
        onValueChange = { name = it },
        label = { Text(text = "Enter Name") },
//        placeholder = {Text(text = "Enter your name")}
        leadingIcon = {
            Icon(
                imageVector = Icons.Default.Person,
                contentDescription = "Person Icon"
            )
        }
    )
    TextField(
        value = passwd,
        onValueChange = {passwd = it},
        label = { Text(text = "Enter password") },
        trailingIcon = {
            Icon(imageVector = Icons.Default.RemoveRedEye, contentDescription = "password icon")
        },
        singleLine = false,
        shape = RoundedCornerShape(15.dp), // circle shape
        colors = TextFieldDefaults.colors(
            focusedTextColor = Color.Blue,
            focusedContainerColor = Color.LightGray

        )
    )
}
```

source code: https://gitlab.com/sharath44665/text-example#


