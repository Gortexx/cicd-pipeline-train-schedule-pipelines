pipeline{
 agent  any
 tools{
    maven 'Maven 3.3.9'
    jdk 'jdk8'
 }
  stages{
    stage ('Initialize'){
      steps {
        echo 'Running build automation'
        sh '''
             echo "PATH = ${PATH}"
             echo "M2_HOME = ${M2_HOME}"
             archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
    stage ('Build'){
      steps {
        echo 'Minimal pipeline'
      }
    }
  }
}
