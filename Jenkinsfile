node {
stage "Checkout"
  checkout scm
stage "Composer"
  sh 'composer install'
stage "Build"
  sh "./vendor/bin/phpunit"
  sh "./vendor/bin/behat"
}
