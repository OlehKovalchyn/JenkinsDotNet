pipeline {
    agent none 
    stages {
        stage('Build') { 
            steps {
                sh 'mcs Hello.cs'
                sh './Hello.exe'
            }   
            }
        }
    }
}
