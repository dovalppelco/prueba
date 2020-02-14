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
				sh 'sudo docker buil <F4><F4>tag=php54local .'	
				sh 'sudo docker images|grep php54local'
			}
		}
	}
}
