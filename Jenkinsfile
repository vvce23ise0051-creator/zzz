pipeline{
  agent any

  tools{
    git 'Git'
    maven 'Maven3'
  }

  stages{
    stage('CHECKOUT'){
      steps{
        git branch :'main' ,url :' https://github.com/vvce23ise0051-creator/zzz.git'
      }
    }
    stage('Build'){
      steps{
        bat 'mvn clean install'
      }
    }
    stage('test'){
      steps{
        dir('demo'){
          bat 'mvn test'
        }
      }
    }
  }
}
