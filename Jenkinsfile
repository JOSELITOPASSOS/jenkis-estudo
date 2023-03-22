pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }

  stages {

	stage('Hello') {

		steps{
			echo "TESTE DEPLOY POR MULTIPLAS BRANCHES"
	  	}
    	}
	
	stage('cat README') {
		
       		when {
			branch "fix-*"
       		}
		
		steps{
			sh java -version
		}
	}

  }

}
