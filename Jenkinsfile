pipeline{
  agent any

  stages{
    stage('Git Clone Repository'){
      steps{
        git branch: "main", url:'https://github.com/AloneX079/newrepo.git'
      }
    }
    stage('Publish HTML'){
      steps{
        publishHTML(target:[
          reportName: 'HTML Page',
          reportDir: '.',
          reportFiles: 'index.html',
          keepAll: true,
          alwaysLinkToLastBuild: true,
          allowMissing: false
        ])
      }
    }
  }
}
