pipeline {
  agent any
  triggers {
    cron('H */2 * * 1-3')
  }
  stages {
    stage('checkout') {
      steps {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'c80f8b91-f836-4663-b42e-20b4f4bad6ef', url: 'https://github.com/rakh-prashant/mavenproject.git']]])
      }
    }
  }
}
