pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }

  stages {

	stage('Fase 01') {

		steps{
			echo "PORCESSOS GERAIS - TODAS AS BRANCHES"
	  	}
    	}
	
	stage('Fase 02') {
		
       		when {
			branch "dev-*"
       		}
		
		steps{
				echo "DEPLOY BRANCH DEVELOP"
		}
	}
	

  }

}
