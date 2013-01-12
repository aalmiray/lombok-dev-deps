This project holds extra build-time dependencies required by the [griffon-lombok-plugin][1] and
dependent plugins. These dependencies must be installed into your local maven repository using
the following command instructions

    mvn install:install-file -DgroupId=org.eclipse.jdt -DartifactId=org.eclipse.jdt.core\
        -Dpackaging=jar -Dversion=3.6.0.v_A58 -Dfile=org.eclipse.jdt.core-3.6.0.v_A58.jar -DgeneratePom=true
    
    mvn install:install-file -DgroupId=org.jetbrains.idea -DartifactId=annotations\
        -Dpackaging=jar -Dversion=11.1.4 -Dfile=annotations-11.1.4.jar -DgeneratePom=true
    
    mvn install:install-file -DgroupId=org.jetbrains.idea -DartifactId=extensions\
        -Dpackaging=jar -Dversion=11.1.4 -Dfile=extensions-11.1.4.jar -DgeneratePom=true
    
    mvn install:install-file -DgroupId=org.jetbrains.idea -DartifactId=util\
        -Dpackaging=jar -Dversion=11.1.4 -Dfile=util-11.1.4.jar -DgeneratePom=true
    
    mvn install:install-file -DgroupId=org.jetbrains.idea -DartifactId=idea-openapi\
        -Dpackaging=jar -Dversion=11.1.4 -Dfile=idea-openapi-11.1.4.jar -DgeneratePom=true

[1]: https://github.com/griffon/griffon-lombok-plugin