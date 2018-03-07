@Library('php-lint')

pipeline {
agent any

node {
stage "Checkout"
  checkout scm
stage "Composer"
  sh 'composer install'
stage "Build"
  sh(libraryResource('com/example/php-lint.sh'))
}
}
