pipeline {
    agent any // Выполнять на любом доступном агенте
    stages {
        stage('Build') {
            steps {
                echo 'Сборка проекта...'
                // Здесь может быть команда, например: sh 'make build'
            }
        }
        stage('Test') {
            steps {
                echo 'Запуск тестов...'
                // Например: sh 'make test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Развертывание...'
                // Например: sh 'make deploy'
            }
        }
    }
    post {
        always {
            echo 'Этот блок выполнится всегда, независимо от результата'
        }
        success {
            echo 'Пайплайн успешно завершен!'
        }
        failure {
            echo 'Что-то пошло не так...'
        }
    }
}
