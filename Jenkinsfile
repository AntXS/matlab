pipeline {
    agent any
    environment {
        PATH = "${PATH}:/Applications/MATLAB_R2020a.app/bin"
    }
    stages {
        stage('Run Tests') {
            steps
            {
                runMATLABTests(
                               testResultsJUnit: 'matlabTestArtifacts/junittestresults.xml'
                               codeCoverageCobertura: 'matlabTestArtifacts/cobertura.xml'
                              )
             }
         }
     }
}
 