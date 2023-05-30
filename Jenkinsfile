def now = new Date()
def today = now.format('YYYY-MM-dd')
def mydate = new Date(system.currentTime())
Calendar date = Calendar.getInstance();
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
                }
            } 
        }
    }
}
