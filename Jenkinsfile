def now = new Date()
today = now.getDay()
numberDay = today.getDay()
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
        
        stage("compare")
        {
            steps
            {
                script
                {
                    def sumar = numero1.toInteger() + numero2.toInteger()
                    println "La suma de los dos numeros es: " + sumar
                    println today
                    println numberDay
                }
                
            }
            
        }
    }
}
