pipeline {

    agent any

    stages {

        stage('SCM') {

            steps {

                      git "https://github.com/NazmurTraining/pipe.git"

                //

            }

        }

        stage('Test') {

            steps {

                         sh "mvn package"

                //

            }

        }

        stage('Deploy1') {

            steps {

                            sh "/sonar_scanner/bin/sonar-scanner"

                //

            }

        }

                                stage('Deploy3') {

            steps {

                               sh "mvn clean deploy"

                //

            }

        }

                                stage('Deploy2') {

            steps {

                   sh 'scp target/*.war root@192.168.1.101:/var/lib/tomcat/webapps/'

                //

            }

        }

    }

}
