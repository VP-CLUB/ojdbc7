# ojdbc7
Oracle JDBC Driver for java oracle.jdbc.driver.OracleDriver ojdbc7

(THIS ARTIFACT IS DEPRECATED, please use a official OTN in your Maven project. Notice here: https://github.com/sgrillon14/MavenSampleOracleJdbc)

# How deploy to sonatype
mvn clean install

unzip .m2\repository\com\oracle\jdbc\ojdbc7\12.1.0.2\ojdbc7-12.1.0.2.jar -d .m2\repository\com\oracle\jdbc\ojdbc7\12.1.0.2\ojdbc7-12.1.0.2

cd ojdbc  (this project directory)

cp .m2\repository\com\oracle\jdbc\ojdbc7\12.1.0.2\ojdbc7-12.1.0.2\oracle target\classes\oracle

cp .m2\repository\com\oracle\jdbc\ojdbc7\12.1.0.2\ojdbc7-12.1.0.2\META-INF target\classes\META-INF

mvn deploy -Pdeploy -Dmaven.main.skip=true -Dmaven.install.skip=true  (configure your Maven setting.xml)

# How use

[![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.github.noraui/ojdbc7/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.github.noraui/ojdbc7)

```xml
<dependency>
    <groupId>com.github.noraui</groupId>
    <artifactId>ojdbc7</artifactId>
    <version>12.1.0.2</version>
</dependency>
```

# License

[![license](https://img.shields.io/github/license/NoraUi/ojdbc7.svg)](https://github.com/NoraUi/ojdbc7/blob/master/LICENSE) + Oracle Technology Network License Agreement, See LICENSE for details

# Contributors

[![GitHub contributors](https://img.shields.io/github/contributors/NoraUi/ojdbc7.svg)](https://github.com/NoraUi/ojdbc7/graphs/contributors)
[![GitHub closed pull requests](https://img.shields.io/github/issues-pr/NoraUi/ojdbc7.svg)](https://github.com/NoraUi/ojdbc7/pulls)
[![GitHub issues](https://img.shields.io/github/issues/NoraUi/ojdbc7.svg)](https://github.com/NoraUi/ojdbc7/issues)
