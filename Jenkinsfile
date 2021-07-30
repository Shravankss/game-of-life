node('GOL') {
    stage('scm') {
   git 'https://github.com/wakaleo/game-of-life.git'
}
stage('build'){
    sh 'mvn clean package'
}
stage('postbuild'){
junit '**/TEST-*.xml'
archive '**/*.war'
}

}