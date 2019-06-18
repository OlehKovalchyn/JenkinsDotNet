pipeline {
    agent none 
    stages {
        stage('Build') { 
            steps {
            msBuild {
            msBuildInstallation('MSBuild 1.8')
            buildFile('./Hello.cs')
            args('check')
            args('another')
            passBuildVariables()
            continueOnBuildFailure()
            unstableIfWarnings()
        }   
            }
        }
    }
}
