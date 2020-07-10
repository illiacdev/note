***
## .jar에 기본 Manifest 속성이 없습니다.

~~~
jar {
    manifest {
        attributes 'Main-Class': 'myfirst.app.App' 
    }
}
~~~

***
## gradle 빌드후 jar 파일 복사, 이름변경

~~~
doLast{
        copy {
            from "${jar.archivePath}"
            into "dist"
            rename { String filename ->
                filename.replace(filename,"app.jar")
            }
        }
    }
~~~
***