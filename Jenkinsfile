def num1 = 2
def num2 = 4
pipeline{
    agent any
    stages{
        stage("Escritura fichero"){
            steps{
                script{
                    def potencia = (num1+num2)*2
                    def multiplicacion = num1 * num2
                    def texto = "El resultado de la potencia es: " + potencia + ", el resultado de la multiplicación es: " + multiplicacion
                    writeFile(file: "resultado.txt", text: texto)
                }
            }
        }
    }
}
