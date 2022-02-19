
pipeline {

    agent any     stages {

        stage('Get Latest Code') {

            steps {

                echo 'Get Latest Code'

                // Get some code from a GitHub repository

                git 'https://github.com/vinoth296/GitlearnbyV.git'

            }

        }

        stage('Clean the Workspace') {

            steps {

                echo 'Clean the Workspace'

                // Run Maven on a Unix agent.

                sh "mvn clean"

            }

        }

        stage('Compile') {

            steps {

                echo 'Compile'

                // Run Maven on a Unix agent.

                sh "mvn clean compile"

            }

        }

        stage('Test') {

            steps {

                echo 'Test'

                // Run Maven on a Unix agent.

                sh "mvn clean compile test"

            }

        }

        stage('Package the Solution') {

            steps {

                echo 'Package the Solution'

                // Run Maven on a Unix agent.

                sh "mvn clean compile package"

            }

        }

    }

}

