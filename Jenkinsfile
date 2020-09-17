pipeline {
  agent any
	
  triggers {
    pollSCM('* * * * *')
  }
	
  stages {
    stage("Compile") {
      steps {
        sh "./Docker compileCode"
      }
    }
  }
	
	 stage("Build") {
      steps {
        sh "./Docker build"
      }
    }
	
	stage("Unit test") {
      steps {
        sh "./Docker test"
      }
    }
}
