job('NodeJS example') {
    scm {
        git('https://github.com/Lovely1207/jenkins-docker-integration-sample.git') {  node -> // is hudson.plugins.git.GitSCM
            node / gitConfigName('DSL User')
            node / gitConfigEmail('kumarilovely1271@gmail.com')
        }
    }
}