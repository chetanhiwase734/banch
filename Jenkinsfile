pipeline {
			agent {
					label{
					
					label "built-in"
					
					
				}
			}

			stages {
			
					stage ("23Q1"){
					
							steps {
							
								sh "docker stop 23Q1"
								sh "docker system prune -a -f"
								sh "docker run -itdp 80:80 --name 23Q1 httpd"
								sh "docker cp /mnt/branch/branch/index.html 23Q1:/usr/local/apache2/htdocs"
					}
			}
			
			stage ("23Q2"){
					steps {
							
								sh "docker stop 23Q2"
								sh "docker system prune -a -f"
								sh "docker run -itdp 90:80 --name 23Q2 httpd"
								sh "docker cp /mnt/branch/branch/index.html 23Q2:/usr/local/apache2/htdocs"
					}
			
			}
			
			stage ("23Q3"){
					steps {
							
								sh "docker stop 23Q3"
								sh "docker system prune -a -f"
								sh "docker run -itdp 100:80 --name 23Q3 httpd"
								sh "docker cp /mnt/branch/branch/index.html 23Q3:/usr/local/apache2/htdocs"
					}
				}
			
			}		
	
}					
