pipeline {
    agent any
    stages {
        stage('Print Hostname') {
            steps {
                sh 'hostname'
            }
        }
        stage('IP Address') {
            steps {
                sh 'hostname -I'
            }
        }
        stage('CPU Details') {
            steps {
                sh 'lscpu'
            }
        }
        stage('Disk Usage') {
            steps {
                sh 'df -kh'
            }
        }
        stage('Memory Usage') {
            steps {
                sh 'free -h'
            }
        }
        stage('Check Jenkins Status') {
            steps {
                sh 'sudo systemctl status jenkins'
            }
        }
    }
}
