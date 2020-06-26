# build.gradle-setting

  
plugins {
    id 'application' 
    id 'com.github.johnrengelman.shadow' version '4.0.4'
}

mainClassName = 'com.thftgr.Main'

version '1.0'
sourceCompatibility = targetCompatibility = 1.8

repositories {
    jcenter()
}


dependencies {
    testCompile group: 'junit', name: 'junit', version: '4.12'
    compile files("${System.properties['java.home']}/../lib/tools.jar")
}

compileJava.options.encoding = 'UTF-8'
