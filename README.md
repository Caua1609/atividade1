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

#### 2.B
```kotlin
fun main() {
    print("Digite a área da obra em m²: ")
    val area = readln().toDouble()

    if (area < 10) {
        println("A obra deve ter no mínimo 10 m² para contratação.")
    } else {
        val mestres = 1
        val serventes = (area / 10).toInt() * 2
        val engenheiros = (area / 100).toInt()

        println("Quantidade de profissionais necessários:")
        println("Mestre de obra: $mestres")
        println("Serventes: $serventes")
        println("Engenheiros: $engenheiros")
    }
}

```
