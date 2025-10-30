pipeline {
    agent any
    tools {
            jdk 'jdk-17' // Jenkins Tools 설정에서 지정한 Name과 정확히 일치해야 합니다.
        }
    stages {
        stage("Compile") {
            steps {
                sh "./gradlew compileJava"
            }
        }
        stage("Build") {
            steps {
                sh "./gradlew build"
            }
        }
        stage("Unit test") {
            steps {
                sh "./gradlew test"
            }
        }
    }
}