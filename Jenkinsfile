pipeline {
  agent { dockerfile true }
  stages {
    stage('Git checkout') {
      steps {
        git branch: 'main', credentialsId: 'ilyataskaev', url: 'https://github.com/SWTec/cppinternship21-phase1.git'
      }
    }
    stage('Test') {
      steps {
       sh '''
          git --version
          curl --version
          cmake --version
          ls -al
        '''
      }
    }
  }
}


