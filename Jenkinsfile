def now = new Date()
def today = now.format('YYYY-MM-dd')
def clima = 18
def habitantes = 180747
def contenido = ""
def num1 = 5
def num2 = 3
pipeline
{
    agent any
    environment
    {
         numero1 = 100
         numero2= 100
    }
    stages
    {
        stage('Bienvenida') 
        {
            steps 
            {
                script 
                {
                    contenido = contenido + "Bienvenid@ hoy es día " + today + "\n"
                    println "Bienvenid@ hoy es día " + today
                }
            } 
        }
        stage('temperatura')
        {
            steps
            {
                script
                {
                    contenido = contenido + "Actualmente en Getafe hacen " + clima + "Cº\n"
                    println "Actualmente en Getafe hacen " + clima + "º"
                }
            }
        }
        stage('calcularPoblacion') 
        {
            steps 
            {
                script {
                    def poblacionNeta = habitantes * 0.8
                    contenido = contenido + "La población neta de Getafe es: " + poblacionNeta + "\n"
                    println "La población neta de Getafe es: " + poblacionNeta
                }
            }
        }
        stage("Sumar")
        {
            steps
            {
                script
                {
                    def sumar = numero1.toInteger() + numero2.toInteger()
                    contenido = contenido + "La suma de los dos numeros es: " + sumar + "\n"
                    println "La suma de los dos numeros es: " + sumar
                }
                
            }
            
        }
        stage("Restar")
        {
            steps
            {
                script
                {
                    def resta = numero1.toInteger() - numero2.toInteger()
                    contenido = contenido + "La resta de los numeros es: " + resta + "\n"
                    println "La resta de los numeros es: " + resta
                }
            }
        }
        stage("Multiplicacion")
        {
            steps
            {
                script
                {
                    def multiplicacion = numero1.toInteger() * numero2.toInteger()
                    contenido = contenido + "La multiplicacion de los numeros es: " + multiplicacion + "\n"
                    println "La multiplicacion de los numeros es: " + multiplicacion
                }
                
            }
        }
        stage("Division")
        {
            steps
            {
                script
                {
                    def division =numero1.toInteger() / numero2.toInteger()
                    if(numero1.toInteger() != 0 && numero2.toInteger() != 0)
                        {
                            contenido = contenido + "La division de los numeros es: " + division + "\n"
                            println "La division de los numeros es: " + division
                        }
                    else
                        {
                            contenido = contenido + "No se puede dividir por 0\n"
                            println "No se puede dividir por 0"   
                        }
                }
            }
        }
        stage('guardado')
        {
            steps
            {
                script
                {
                    println "Se va a guardar en un fichero el siguiente contenido: \n" + contenido
                    writeFile(file: "salida.txt", text:contenido)
                }
            }
        }
    }
}
