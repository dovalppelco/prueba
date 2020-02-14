pipeline {
	agent any
	stages{
		stage('Primera inicialización')
		{
			steps{
				sh 'echo inicializando...'
			}	
		}
		stage ('Checando Docker'){
			steps {
				sh 'sudo docker ps'
			}
		}
	}
}
