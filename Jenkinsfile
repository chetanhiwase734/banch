pipeline {
			agent {
					label{
					
					label "built-in"
					
					
				}
			}

			stages {
			
					stage ("23Q2"){
					
							steps {
							
								sh "docker stop 23Q1"
								sh "docker system prune -a -f"
								sh "docker run -itdp 90:80 --name 23Q2 httpd"
								sh "docker cp /mnt/branch/branch/index.html 23Q1:/usr/local/apache2/htdocs"
					}
			}
		}	
}
