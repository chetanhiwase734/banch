pipeline {
			agent {
					label{
					
					label "built-in"
				
					
				}
			}

			  stages { 
			
					stage ("23Q1"){
					
							steps {
								sh "cd /mnt/branch/branch"
								sh "docker stop 23Q1"
								sh "docker system prune -a -f"
								sh "git checkout 23Q1"
								sh "docker run -itdp 80:80 --name 23Q1 httpd"
								sh "docker cp index.html 23Q1:/usr/local/apache2/htdocs"
								
					}
			}
		}	
}
