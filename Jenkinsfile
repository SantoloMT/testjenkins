pipeline {
  agent any

  stages{

      stage("build") {
        steps {
          echo 'Building the application...'
          sh '''
          cd myapp
          pip install -r requirements.txt
          '''
          
        }
      }
      stage('Test') {
      steps {
        echo 'Testing...'
        sh '''
        cd myapp
        python3 hello.py
        python3 hello.py --name=Brad
        '''
  }
      }
  }
    
}
