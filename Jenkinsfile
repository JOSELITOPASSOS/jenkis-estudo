pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }

  stages {

	stage('Fase 01') {

		steps{
			echo "TESTE DEPLOY POR MULTIPLAS BRANCHES"
	  	}
    	}
	
	stage('Fase 02') {
		
       		when {
			branch "fix-*"
       		}
		
		steps{
			java -version
		}
	}
	

  }

}
