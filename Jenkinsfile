pipeline {
    agent { label 'master' }
    parameters {
        string(name: 'Hello', defaultValue: 'Greetings', description: 'How should I greet the world?')
        string(name: 'FirstOption', defaultvalue: "test")
        string(name: 'AnotherOption', defaultvalue: "test12")
        
    }
    stages {
        stage('build') {
            steps {
                echo "${params.Hello} World!"
            }
        }
    }
}
