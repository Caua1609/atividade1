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

### Atividade 2
#### 2.A
```kotlin
fun main() {
    print("Digite o comprimento de um dos lados do terreno (m): ")
    val lado1 = readln().toFloat()

    print("Digite o segundo valor (m): ")
    val lado2 = readln().toFloat()

    val area = lado1 * lado2

    print("A área do terreno é de: $area m²")
}

```
