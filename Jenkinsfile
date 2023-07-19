pipeline {
			agent {
					label{
					
					label "built-in"
					
					
				}
			}

			stages {
			
					stage ("23Q3"){
					
							steps {
							
								sh "docker stop 23Q3"
								sh "docker system prune -a -f"
								sh "docker run -itdp 100:80 --name 23Q3 httpd"
								sh "docker cp /mnt/branch/branch/index.html 23Q3:/usr/local/apache2/htdocs"
								sh "docker exec -itdp 100:80 --name 23Q3 httpd"
					}
			}
		}	
}
