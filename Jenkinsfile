pipeline {
    agent any

    stages {
        stage('Apt update') {
            steps {
                // Install MariaDB on Ubuntu
                sh 'sudo apt-get update -y'
                     }
        }
        stage('Install MariaDB') {
            steps {
         
                sh 'sudo apt-get install -y mariadb-server'
            }
        }
        stage(' MariaDB Version') {
            steps {
            // Display Maven version
                sh 'sudo systemctl status mariadb'
            }
        }
    }
}
