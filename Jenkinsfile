 stage('Build'){

            steps {

                bat "mvn clean install -DskipTests"

            }

        }

 
pipeline {

    agent any

    tools{

        maven 'maven'

        jdk 'jdk-11'

    }

 

    stages {

    stage('Git checkout') {

            steps {

                git branch: 'main', credentialsId: 'github_credential', url: ' stage('Build'){

            steps {

                bat "mvn clean install -DskipTests"

            }

        }

 
pipeline {

    agent any

    tools{

        maven 'maven'

        jdk 'jdk-17'

    }

 

    stages {

    stage('Git checkout') {

            steps {

                git branch: 'main', credentialsId: 'github_credential', url: 'https://github.com/Nissi-1314/Payment-Service.git
'

            }

        }

 

 

        stage('Test') {

            steps {

                bat 'mvn test'

            }

        }

        stage('SonarQube Analysis') {

            steps {

                    bat 'mvn org.sonarsource.scanner.maven:sonar-maven-plugin:3.8.0.2131:sonar -Dsonar.login=admin -Dsonar.password=Nissi@1314'

                }

        }

 

 

 

       stage("Deployment") {

           steps{

    bat 'start /B mvnw spring-boot:run -Dserver.port=8001'

}

       }

    }

}'

            }

        }

 

 

        stage('Test') {

            steps {

                bat 'mvn test'

            }

        }

        stage('SonarQube Analysis') {

            steps {

                    bat 'mvn org.sonarsource.scanner.maven:sonar-maven-plugin:3.8.0.2131:sonar -Dsonar.login=admin -Dsonar.password=Nissi@1314'

                }

        }

 

 

 

       stage("Deployment") {

           steps{

    bat 'start /B mvnw spring-boot:run -Dserver.port=8001'

}

       }

    }

}
