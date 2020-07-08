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
## gradle 빌드후 jar 파일 복사

~~~
jar {
 
    doLast{
        copy {
            from "${jar.archivePath}"
            into "target/dist"
        }

    }
}
~~~
***