# Atividades

### Atividade 1 (IMC)
```kotlin
fun main() {
    print("Digite o peso: ")
    val peso = readln().toDouble()

    print("Digite a altura: ")
    val altura = readln().toDouble()

    val imc = peso / (altura * altura)

    if (imc < 18.5) {
        print("Abaixo do peso")
    } else if (imc < 24.9) {
        print("Peso normal")
    } else if (imc < 29.9) {
        print("Sobrepeso")
    } else {
        print("Obesidade")
    }
}

```
