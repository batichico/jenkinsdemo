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
        
        stage("Sumar")
        {
            steps
            {
                script
                {
                    def sumar = numero1.toInteger() + numero2.toInteger()
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
                println "La division de los numeros es: " + division
                    }
                else
                {
                 println "No se puede dividir por 0"   
                }
            }
        }
        }
    }
}
