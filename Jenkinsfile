pipeline {
    agent any    
    stages {
        stage('install pkgs') { 
            steps {
               echo "install nginx application"
               sudo apt-get install nginx -y
            }
        }
        stage('configure appln') { 
            steps {
                echo "this is test stage"
                systemctl start nginx
                systemctl enable nginx
            }
        }
        stage('web-page') { 
            steps {
                echo "this is test deploymment1"
                sudo cp /home/ubuntu/2095_level/ /var/www/html
            }
        }
        stage('Deployment') { 
            steps {
                echo "this is test deploymment2"
            }
        }
    }
}
