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

#### 2.C
```kotlin
fun main() {
    print("Informe a área da obra em m²: ")
    val area = readLine()!!.toDouble()

    print("Quantidade de quartos sem suíte: ")
    val quartoSemSuite = readLine()!!.toInt()

    print("Quantidade de quartos com suíte: ")
    val quartoComSuite = readLine()!!.toInt()

    print("Quantidade de banheiros: ")
    val banheiros = readLine()!!.toInt()

    print("Quantidade de áreas de serviço: ")
    val areaServico = readLine()!!.toInt()

    print("Quantidade de piscinas: ")
    val piscina = readLine()!!.toInt()

    val valorPorArea = (area / 10) * 4500
    val valorQuartoSemSuite = quartoSemSuite * 12000
    val valorQuartoComSuite = quartoComSuite * 17000
    val valorBanheiro = banheiros * 5000
    val valorAreaServico = areaServico * 15000
    val valorPiscina = piscina * 27550

    val valorTotal = valorPorArea +
            valorQuartoSemSuite +
            valorQuartoComSuite +
            valorBanheiro +
            valorAreaServico +
            valorPiscina

    println("O valor total da obra é de R$ $valorTotal,00")
}

```

#### 2.D
```kotlin
fun main() {
    print("Quantidade de mestres na obra: ")
    val mestre = readLine()!!.toInt()

    print("Quantidade de serventes na obra: ")
    val serventes = readLine()!!.toInt()

    print("Quantidade de engenheiros na obra: ")
    val engenheiros = readLine()!!.toInt()

    val valorMestre = 3500.0
    val valorServente = 1900.0
    val valorEngenheiro = 11000.0

    val totalMestre = mestre * valorMestre
    val totalServente = serventes * valorServente
    val totalEngenheiro = engenheiros * valorEngenheiro

    val valorTotal = totalMestre + totalServente + totalEngenheiro

    println("O valor total da mão de obra é de R$ $valorTotal,00")
}
```

#### 2.E
```kotlin
fun main() {

print("Área da obra (m²): ")
val area = readLine()!!.toDouble()

print("Quartos sem suíte: ")
val quartosSemSuite = readLine()!!.toInt()

print("Quartos com suíte: ")
val quartosComSuite = readLine()!!.toInt()

print("Banheiros: ")
val banheiros = readLine()!!.toInt()

print("areaServiço: ")
val areaServico = readLine()!!.toInt()

print("piscinas: ")
val piscina = readLine()!!.toInt()

val blocos10m2 = area / 10
val subtotalArea = blocos10m2 * 4500
val subtotalQuartosSemSuite = quartosSemSuite * 12000
val subtotalQuartosComSuite = quartosComSuite * 17000
val subtotalBanheiros = banheiros * 5000
val subtotalAreaServico = areaServico * 15000
val subtotalPiscina = piscina * 27550

val totalSemMaoDeObra = subtotalArea +
subtotalQuartosSemSuite +
subtotalQuartosComSuite +
subtotalBanheiros +
subtotalAreaServico +
subtotalPiscina

print("\nQuantidade de mestres de obra: ")
val mestres = readLine()!!.toInt()

print("Quantidade de serventes: ")
val serventes = readLine()!!.toInt()

print("Quantidade de engenheiros: ")
val engenheiros = readLine()!!.toInt()

val custoMaoDeObra =
(mestres * 3500) +
(serventes * 1900) +
(engenheiros * 11000)

val totalComMaoDeObra = totalSemMaoDeObra + custoMaoDeObra
val lucroEmpresa = totalComMaoDeObra * 0.25
val valorFinalCliente = totalComMaoDeObra + lucroEmpresa
val custoFinalObra = totalComMaoDeObra - custoMaoDeObra

println("\n========== RELATÓRIO DA OBRA ==========")
println("Subtotal por área: R$ $subtotalArea")
println("Quartos sem suíte: R$ $subtotalQuartosSemSuite")
println("Quartos com suíte: R$ $subtotalQuartosComSuite")
println("Banheiros: R$ $subtotalBanheiros")
println("Área de serviço: R$ $subtotalAreaServico")
println("Piscina: R$ $subtotalPiscina")

println("\nTotal da obra (sem mão de obra): R$ $totalSemMaoDeObra")
println("Total da mão de obra: R$ $custoMaoDeObra")
println("Total da obra (com mão de obra): R$ $totalComMaoDeObra")

println("\nLucro da empresa (25%): R$ $lucroEmpresa")
println("Valor final a receber: R$ $valorFinalCliente")
println("Custo da obra (descontando folha): R$ $custoFinalObra")
}

```
