pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'echo "Hello World"'
                withMaven(maven:'Maven Install',mavenSettingsConfig:'mavensettings.xml'){
                 bat 'mvn -DskipTests clean package'
                 }
            }
        }
    }
}
