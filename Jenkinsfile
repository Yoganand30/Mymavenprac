pipeline{
  agent any
  tools{
    maven 'Maven'
  }
  stages{
    stage('checkout'){
      steps{
        git barnch:'master',url:'https://github.com/Yoganand30/Mymavenprac.git'
      }
    }
  stage('Build'){
    steps{
      sh 'mvn complie package'
    }
  }
  stage('test'){
    steps{
      sh 'mvn test'
    }
  }
  stage('run'){
    steps{
      sh 'java -jar target/mavenpra-1.0-SNAPSHOT.jar'
    }
  }
  }
}
