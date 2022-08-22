# Links
* Home page: https://hibernate.org/
* ORM: https://hibernate.org/orm/
* Documentation: https://hibernate.org/orm/documentation/5.6/ 
    - Getting Started Guide: https://docs.jboss.org/hibernate/orm/5.6/quickstart/html_single/
        + Hibernate Download: https://sourceforge.net/projects/hibernate/files/hibernate-orm/
    - User Guide: https://docs.jboss.org/hibernate/orm/5.6/userguide/html_single/Hibernate_User_Guide.html
    - Integration Guide: https://docs.jboss.org/hibernate/orm/5.6/integrationguide/html_single/Hibernate_Integration_Guide.html

# Source Code
The original source code is from **Hibernate Download**, unzip it, workspace/hibernate-release-5.6.5.Final/documentation/quickstart/html_single/hibernate-tutorials. Explanation is: https://docs.jboss.org/hibernate/orm/5.6/quickstart/html_single/ which covers 

* Tutorial Using Native Hibernate APIs and hbm.xml Mapping
    - basic
* Tutorial Using Native Hibernate APIs and Annotation Mappings
    - annotations
* Tutorial Using the Java Persistence API (JPA)
    - entitymanager
* Tutorial Using Envers
    - envers

    
# Other tutorial
https://www.youtube.com/watch?v=KHohVibqePw

Hibernate and MySQL: 

```xml
<?xml version="1.0" encoding="UTF-8"?>
<persistence version="2.1" xmlns="http://xmlns.jcp.org/xml/ns/persistence"
             xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
             xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/persistence
             http://xmlns.jcp.org/xml/ns/persistence/persistence_2_1.xsd">
    <persistence-unit name="org.hibernate.tutorial.jpa">

        <properties>
            <property name="hibernate.connection.driver_class" value="com.mysql.jdbc.Driver"/>
            <property name="hibernate.connection.url" value="jdbc:mysql://localhost:3306/classicmodels"/>
            <property name="hibernate.connection.autocommit" value="false"/>
            <property name="hibernate.connection.username" value="root"/>
            <property name="hibernate.connection.password" value=""/>
            <property name="hibernate.dialect" value="org.hibernate.dialect.MySQL5Dialect"/>
            <property name="hibernate.connection.CharSet" value="utf8"/>
            <property name="hibernate.connection.characterEncoding" value="utf8"/>
            <property name="hibernate.connection.useUnicode" value="true"/>
            <property name="hibernate.show_sql" value="true"/>
            <property name="hibernate.hbm2ddl.auto" value="update"/>
            <!-- use encache provider-->
            <!--<property name="hibernate.cache.region.factory_class"-->
            <!--value="org.hibernate.cache.ehcache.EhCacheRegionFactory"/>-->
            <!--<property name="hibernate.javax.cache.provider" value="org.ehcache.jsr107.EhcacheCachingProvider"/>-->
            <!--&lt;!&ndash;use second level cache&ndash;&gt;-->
            <!--<property name="hibernate.cache.use_second_level_cache" value="true"/>-->
            <!--&lt;!&ndash;use 3rd level cache&ndash;&gt;-->
            <!--<property name="hibernate.cache.use_query_cache" value="true"/>-->
        </properties>
    </persistence-unit>
</persistence>
```

## TODO
Follow the above tutorial to create a example for MySQL