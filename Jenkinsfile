pipeline {

    agent any
  
    stages {
        stage('Construir') {
            when {
                branch 'main'
            }

            steps {
                echo "Construye solo con la rama Main"
            }
        }

        stage('Pruebas') {
            when {
                not {
                    branch 'develop'
                }
            }

            steps {
                echo "Ejecute las pruebas condicionales con la rama que no sea develop"
            }
        }
    }
}