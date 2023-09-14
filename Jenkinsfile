pipeline {
    agent any
    tools {
        gradle "Gradle 8.3"
    }
    stages {
        stage ('clone') {
            steps {
                sh 'git clone https://github.com/MrMiano-DevOps/java-todo.git'
                
                echo "cloning complete"
            }
        }
        
        stage ('build') {
            steps {
                sh 'gradle build'
                
                echo "build complete"
            }
        }
        
        stage ('test') {
            steps {
                sh 'gradle test'
                
                echo "testing complete"
            }
        }
    }
}
