#!/usr/bin/env groovy
pipeline {
         agent any
         stages {
                 stage('One') {
                    steps {
                      echo 'Olá estou testando!!'
                    }
                 }
                 stage('Build') {
                 steps {                                           
                      echo 'cd GOPATH'
                      sh 'cd C:/desenvolvimentoGo/src/github.com/CezarGarrido/go-jenkins-example/ && go build'            
                   }     
                 }
               }
}