def fichero = "C:\\ProgramData\\Jenkins\\.jenkins\\userContent\\prueba3.txt"

pipeline
{
    agent any
    stages
    {
        stage("Creacion de fichero")
        {
            steps
            {
                script
                {
                  def cadena = "Esperando finales de junio para ir a Bilbao y ver en concierto a Joaquin Sabina"
                  writeFile file: fichero, text: cadena
                }
            }
        }
		stage("Lectura de fichero")
        {
            steps
            {
                script
                {
					def lectura = readFile fichero
					println lectura
                }
            }
        }
    }  
}
