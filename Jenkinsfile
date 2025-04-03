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
                    reportDir: 'reports',
                    reportFiles: 'index.htm',
                    reportName: 'Build Report'
                ])
            }
        }
    }
}
