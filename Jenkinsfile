import java.text.SimpleDateFormat
pipeline
{
    agent any
    stages
    {
        stage("Fecha")
        {
            steps
            {
                script
                {
                    dia = new Date().getDay()
                    dia_actual = new Date()
                    formato = new SimpleDateFormat("dd/MM/yyyy HH:mm:ss")
                    fechaConFormato = formato.format(dia_actual)
                    mapa = [1: "Lunes", 2: "Martes", 3: "Miercoles", 4: "Jueves", 5: "Viernes", 6: "Sabado", 7: "Domingo"]
                    println "El dia actual es: " + mapa[dia]
                    println "La fecha con el nuevo formato es: " +fechaConFormato
                }
            }
        }
    }
}
