pipeline{
    agent{label 'master'}
    tools{maven 'M3'}
    stages{
        stage('Checkout'){
            steps{
                git branch: 'master', url: 'https://github.com/machredd/front-end.git'
            }
        }
        stage('Build'){
            tools{
                jdk 'JAVA_HOME'
            }
            steps{
                bat 'mvn compile'
            }
        }
        stage('Package'){
            tools{
                jdk 'JAVA_HOME'
            }
            steps{
                bat 'mvn package'
            }
        }
         stage('Deploy'){
      steps{
bat 'Java -jar C:\Users\MACHREDD\OneDrive - Capgemini\Desktop\ECommerce-Angular-Spring-master (1)\ECommerce-Angular-Spring-master\frontend.jar'
        
        }
    }
}
}
