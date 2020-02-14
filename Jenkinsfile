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
		stage ('Construir imagen')
		{
			steps {
				sh 'sudo docker build  --tag=php54local .'	
				sh 'sudo docker images|grep php54local'
			}
		}
		stage ('Desplegar')
		{
			steps {
				sh 'echo docker-compose.yml'
			}
		}
	}
}
