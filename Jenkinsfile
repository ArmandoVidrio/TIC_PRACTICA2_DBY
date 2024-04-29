pipeline {
    agent any // Define el agente de Jenkins que ejecutará el pipeline (puede ser 'any', 'node', 'docker', etc.)

    stages { // Define las etapas del pipeline
        stage('Preparación') { // Etapa de preparación
            steps {
                // Pasos o comandos a ejecutar en esta etapa
                echo 'Iniciando el pipeline despues de recibir la notificacion de los cambios..'
            }
        }

        stage('Construcción') { // Etapa de construcción
            steps {
                // Pasos de construcción (compilar código, ejecutar pruebas, etc.)
                echo 'Construyendo el proyecto...'
            }
        }

        stage('Despliegue') { // Etapa de despliegue
            steps {
                // Pasos de despliegue (desplegar aplicación, notificar, etc.)
                echo 'Desplegando la aplicación...'
            }
        }
    }

    post { // Define acciones a realizar después de ejecutar todas las etapas
        always {
            // Acciones a realizar siempre, independientemente del resultado del pipeline
            echo 'Pipeline completado.'
        }
        success {
            // Acciones a realizar si el pipeline se ejecuta con éxito
            echo 'El pipeline se ejecutó con éxito.'
        }
        failure {
            // Acciones a realizar si el pipeline falla
            echo 'El pipeline falló.'
        }
    }
}
