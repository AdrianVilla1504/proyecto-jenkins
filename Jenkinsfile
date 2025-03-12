pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Clonando el repositorio...'
                git 'https://github.com/AdrianVilla1504/proyecto-jenkins.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Ejecutando la fase de Build...'
                sh 'echo "Compilación simulada completada"'
            }
        }

        stage('Test') {
            steps {
                echo 'Ejecutando pruebas...'
                sh 'echo "Pruebas ejecutadas exitosamente"'
            }
        }

        stage('Deploy Simulation') {
            steps {
                echo 'Simulando despliegue...'
                sh 'echo "Despliegue simulado completado"'
            }
        }
    }

    post {
        success {
            echo 'Pipeline ejecutado correctamente'
        }
        failure {
            echo 'Error en el pipeline'
        }
    }
}