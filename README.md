maven customer plugin demo

# command

mvn archetype:generate with number 1459
mvn install
mvn org.sonatype.mavenbook.plugins:first-maven-plugin:1.0-SNAPSHOT:echo
mvn org.sonatype.mavenbook.plugins:first-maven-plugin:1.0-SNAPSHOT:echo -Decho.message="The Eagle has Landed"


add this to your ~/.m2/setting.xml:

<pluginGroups>
        <pluginGroup>org.sonatype.mavenbook.plugins</pluginGroup>
</pluginGroups>

/usr/libexec/java_home
export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_231.jdk/Contents/Home

# This goovy plugin can be executed under maven 2.2.1, but not under maven 3.

firstgroovy-maven-plugin mvn --version
Apache Maven 2.2.1 (r801777; 2009-08-06 12:16:01-0700)
Java version: 1.8.0_231
Java home: /Library/Java/JavaVirtualMachines/jdk1.8.0_231.jdk/Contents/Home/jre
Default locale: en_US, platform encoding: UTF-8
OS name: "mac os x" version: "10.14.6" arch: "x86_64" Family: "mac"

mvn firstgroovy:echo

mvn firstgroovy:echo -Decho.message="mymessage"


