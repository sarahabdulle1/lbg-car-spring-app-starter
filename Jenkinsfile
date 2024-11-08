pipeline{
  agent any
  stages {
      stage ('Checkout'){
          steps{
            git branch: 'main', url:'https://github.com/sarahabdulle1/lbg-car-spring-app-starter.git'
          }
      }

      stage ('Install'){
          steps {
            sh "mvn install"
          }
      }

      stage ('Compile'){
          steps {
            sh "mvn clean compile"
          }
      }
      stage ('Test'){
          steps {
            sh "mvn test"
          }
      }    
    //Docker Build Stage, Tag Image, Build Image, Push Image
    }
  }
