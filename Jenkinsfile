pipeline {
    agent { label 'master' }
    parameters {
        string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
    }
    stages {
        stage('build') {
            steps {
                echo "${params.Greeting} World!"
            }
        }
    }
}
