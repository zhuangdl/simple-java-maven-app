pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('GetCode') {
      steps {
        sleep 5
      }
    }
    stage('build') {
      steps {
        mvn_home=tool "mvn"
        sh '${mvn_home}/bin/mvn clean install -DskipTests'
      }
    }
  }
}
