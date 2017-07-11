withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: 'MyID', usernameVariable: 'GIT_USERNAME', passwordVariable: 'GIT_PASSWORD']]) {

    sh("git tag -a some_tag -m 'Jenkins'")
    sh("git push https://${env.GIT_USERNAME}:${env.GIT_PASSWORD}@<REPO> --tags")
}
