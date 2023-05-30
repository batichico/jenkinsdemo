def now = new Date()
def today = now.format('YYYY-MM-dd')
def mydate = new Date(system.currentTime())
def clima = 18
pipeline
{
    agent any
    stages
    {
        stage('compareDay') 
        {
            steps 
            {
                script 
                {
                    if(mydate == 1)
                    {
                        println "Hoy es lunes"
                    }
                    if(mydate == 2)
                    {
                        println "Hoy es martes"
                    }
                    if(mydate == 3)
                    {
                        println "Hoy es miércoles"
                        println "Actualmente en Getafe hacen " + clima + "º"
                    }
                    if(mydate == 4)
                    {
                        println "Hoy es jueves"
                        git branch: "main", url: "https://github.com/samuelegoitz/jenkinsdemo.git"
                    }
                    if(mydate == 5)
                    {
                        println "Hoy es Viernes"
                    }
                    if(mydate == 6)
                    {
                        println "Hoy es Sabado"
                    }
                    if(mydate == 7)
                    {
                        println "Hoy es Domingo"
                    }
                    
                }
            } 
        }
    }
}
