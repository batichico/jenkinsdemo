def now = new Date()
def today = now.getDay()
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
                    if(today == 1)
                    {
                        println "Hoy es lunes"
                    }
                    if(today == 2)
                    {
                        println "Hoy es martes"
                        println "El usuario es " + env.USERNAME
                    }
                    if(today == 3)
                    {
                        println "Hoy es miércoles"
                        println "Actualmente en Getafe hacen " + clima + "º"
                    }
                    if(today == 4)
                    {
                        println "Hoy es jueves"
                        git branch: "main", url: "https://github.com/samuelegoitz/jenkinsdemo.git"
                    }
                    if(today == 5)
                    {
                        println "Hoy es Viernes"
                    }
                    if(today == 6)
                    {
                        println "Hoy es Sabado"
                    }
                    if(today == 7)
                    {
                        println "Hoy es Domingo"
                    }
                }
                
            }
            
        }
    }
}
