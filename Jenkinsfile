pipeline{
agent{
	label 'build-in'

}

	stages{
		stage('install apache'){
			steps{
				sh 'yum install httpd -y'
			}
		}
		stage('start apache'){
			steps{
				sh 'service httpd start'
			}
		
		}
		stage ('deploy apache'){
			steps{
				sh 'cp -r index.html /var/wwww/html'
				sh 'chmod -R 777 /var/www/html/index.html'

			}

		}


	}
}
