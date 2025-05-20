pipeline {
    agent any
    stages {
        stage('Clonar Repositório') {
            steps {
                echo 'Clonando o repositório...'
            }
        }
        stage('Build') {
            steps {
                echo 'Executando build do projeto...'
                echo 'Deploy da Vinheria - Catálogo e Pedidos'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Simulando deploy para a pasta de publicação...'
                bat 'mkdir C:\\vinheria\\catalogo'
                bat 'mkdir C:\\vinheria\\pedidos'
                bat 'copy catalogo\\index.js C:\\vinheria\\catalogo\\index.js'
                bat 'copy pedidos\\index.js C:\\vinheria\\pedidos\\index.js'
            }
        }
    }
}