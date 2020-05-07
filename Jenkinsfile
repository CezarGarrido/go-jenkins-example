#!/usr/bin/env groovy
pipeline {
         agent any
         stages {
                 stage('One') {
                    steps {
                      echo 'Hi, this is Zulaikha from edureka'
                    }
                 }
                 stage('Two') {
                 steps {                                           
                    // Create our project directory.
                      echo 'cd GOPATH'
                      sh 'cd ${GOPATH}/src'
                      echo 'mkdir GOPATH'
                      sh 'mkdir -p ${GOPATH}/src/github.com/CezarGarrido/go-jenkins-example'
                      // Copy all files in our Jenkins workspace to our project directory.   
                      echo 'cp GOPATH'             
                      sh 'cp -r ${WORKSPACE}/* ${GOPATH}/src/CezarGarrido/go-jenkins-example'
                      // Copy all files in our "vendor" folder to our "src" folder.
                      sh 'cp -r ${WORKSPACE}/vendor/* ${GOPATH}/src'
                      // Build the app.
                      sh 'go build'               
                   }     
                 }
               }
}