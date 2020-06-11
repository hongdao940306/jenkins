#!/bin/bash

node {  
   stage('enter android_build'){
       sh 'cd android_build'
       echo 'enter android_build'
   }
    stage('build'){
        echo 'source build/envsetup.sh'
        sh 'source build/envsetup.sh '
        echo 'lunch tti_g1-eng'
        sh 'lunch tti_g1-eng'
        echo 'start to build eng'
        sh 'make 2>&1  -j8 | tee eng.log'
        echo 'finish'
   }
}
