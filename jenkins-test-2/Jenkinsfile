pipeline {
  agent any

  options {
     timestamps()
     disableConcurrentBuilds()
     timeout(time: 2, unit: 'HOURS') 
  }

  parameters {
    string(
      name: 'YOURNAME', 
      defaultValue: 'world', 
      description: 'Name to greet'
    )
  }

  stages {

    stage('Say Goodbye') {
        steps {
          echo "Goodbye ${env.YOURNAME}.  Everything sucks!"
        }
    }
  }

}
