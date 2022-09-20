pipeline {
    agent { label 'master' }
    parameters {
        string(name: 'Hello', defaultValue: 'Greetings!', description: 'How should I greet the world?')
        string(name: 'FirstOption', defaultValue: 'test1', description: '1st Option')
        string(name: 'SecondOption', defaultValue: 'test2', description: '2nd Option')
    }
    stages {
        stage('build') {
            steps {
                echo "${params.Hello} World!"
                echo "${params.FirstOption} First1st!"
                echo "${params.AnotherOption} second2nd!"
            }
        }
    }
}
