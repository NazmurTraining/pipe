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

                            sh "/sonar_scanner/bin/"

                //

            }

        }

                                stage('Deploy3') {

            steps {

                                                echo "this is step1"

                //

            }

        }

                                stage('Deploy2') {

            steps {

                                                echo "this is step1"

                //

            }

        }

    }

}
