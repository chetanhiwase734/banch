pipeline {
			agent {
					label{
					
					label "built-in"
					
					
				}
			}

			  stages {
			
					stage ("23Q2"){
					
						steps {
							
								sh "cd /mnt/branch/branch"
								
								sh "docker system prune -a -f"
								sh "git checkout 23Q2"
								sh "docker run -itdp 90:80 --name 23Q1 httpd"
								sh "docker cp index.html 23Q2:/usr/local/apache2/htdocs"
								sh "docker exec 23Q2 chmod -R 777 /usr/local/apache2/htdocs/index.html"
								
					}
			}
		}	
}
