pipeline {
  agent {label 'agent1'}
  stages {
    stage('Build') {
      steps {
        sh 'echo dev-1231 builds'
      }
    }
  }
  post{
                always {
                    echo(message: 'This is test stage')
                    
                }
                unsuccessful {
                    echo(message: 'test stage is unsuccessfull')
                    
                }
                success{
                    echo(message: 'test stage is successfull')
                }
                failure{
                    echo(message: 'test stage is failure')
                }

            }
}
