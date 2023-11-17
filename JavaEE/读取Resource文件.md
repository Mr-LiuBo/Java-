## ResourceUtils

```java
File file = ResourceUtils.getFile("classpath:temp/client.properties")
Properties p = new Properties();  
p.load(FileUtils.openInputStream(file));
String f5Url = p.getProperty("f5Url");
```



## ClassPathResource

```java
ClassPathResource classPathResource = new ClassPathResource( "temp/client.properties" );
Properties p = new Properties();
p.load(classPathResource.getInputStream());
String f5Url = p.getProperty("f5Url");
```

