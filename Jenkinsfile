def num1 = 2
def num2 = 4
pipeline{
    agent any
    stages{
        stage("Escritura fichero"){
            steps{
                script{
                    def potencia = (num1+num2)*(num1+num2)
                    def multiplicacion = num1 * num2
                    def texto = "El resultado de la potencia es: " + potencia + ", el resultado de la multiplicación es: " + multiplicacion
                    writeFile(file: "resultado.txt", text: texto)
                    println "Número 1: " + num1
                    println "Número 2: " + num2
                    println "El resultado de la potencia es: " + potencia
                    println "El resultado de la multiplicación es: " + multiplicacion
                }
            }
        }
    }
}
