pipeline {
  agent any
  
  stages {
    stage('Checkout') {
      steps {
        git branch: 'main', url: 'https://github.com/anish612/hello-world-react-native-app.git'
      }
    }
    stage('Build') {
      steps {
        sh 'npm install'
        sh 'npm run build'
        sh 'npm run android:release'
      }
    }
  }
}
