# Experiências em Kotlin
Neste arquivo serão adicionados experimentos básicos em Kotlin

## Repetição com exclusão
Este trecho imprime todos os números páres de 0 a 100

##
fun main() {
    for(i in 2 until 102 step 2){
        if (i < 100) print("$i, ")
        else print("$i.")
        if (i % 10 == 0) print("\n")
    }
}
##

## Exemplo de when extraido da documentação oficial

##
fun main() {
    cases("Hello")
    cases(1)
    cases(0L)
    cases(MyClass())
    cases("hello")
}

fun cases(obj: Any) {
    when (obj) {
        1 			-> println("One")
        "Hello" 	-> println("Greeting")
        is Long 	-> println("Long")
        !is String 	-> println("Not is string")
        else 		-> println("Unknown")
    }
}

class MyClass
