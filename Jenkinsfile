pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                echo 'Publishing HTML'
                publishHTML(target: [
                    allowMissing: false,
                    alwaysLinkToLastBuild: true,
                    keepAll: true,
                    reportDir: '.',
                    reportFiles: 'index.html',
                    reportName: 'Build Report'
                ])
            }
        }
    }
}
