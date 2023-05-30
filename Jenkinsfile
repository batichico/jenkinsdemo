def mydate = new Date(system.currentTime())
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
                    println mydate
                }
                
            }
            
        }
    }
}
