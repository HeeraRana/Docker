pipeline {
  agent any
      stages {
      stage("Build") {
      steps {
	      echo 'Building the solution'
        sh "./Docker build"
      }
    }
  }
}
