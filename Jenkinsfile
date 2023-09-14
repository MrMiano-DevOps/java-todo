pipeline {
    agent any
    tools {
        gradle "Gradle-6"
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
                gradle build
                
                echo "build complete"
            }
        }
        
        stage ('test') {
            steps {
                gradle test
                
                echo "testing complete"
            }
        }
    }
}
