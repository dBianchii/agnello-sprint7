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
                sh 'mkdir -p /vinheria/catalogo'
                sh 'mkdir -p /vinheria/pedidos'
                sh 'cp catalogo/index.js /vinheria/catalogo/index.js'
                sh 'cp pedidos/index.js /vinheria/pedidos/index.js'
            }
        }
    }
}