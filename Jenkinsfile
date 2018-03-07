node {
stage "Checkout"
  checkout scm
stage "Composer"
  sh 'composer install'
stage "Build"
  sh "phpunit"
  sh "behat"
}
