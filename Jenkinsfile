pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'hello'
	echo 'world'
      }
    }
    stage('cat README'){
	when {
	branch "fix-*'
	}
	steps{

	sh '''
	   cat README.md
	   '''
	}
    }
  }
}
