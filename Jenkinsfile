pipeline{
  agent none
   steps{
   msBuild {
      msBuildInstallation('MSBuild 1.8')
            buildFile('./HelloWorld.cs')
            args('check')
            args('another')
            passBuildVariables()
            continueOnBuildFailure()
            unstableIfWarnings()
   }
   }
}
