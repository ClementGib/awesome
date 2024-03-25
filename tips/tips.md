## CORE
- classpath : included directories where find classes and packages
  - `target/classes`
  - `target/test-classes`
  - `target/lib`
  - `target/dependency`
  - `src/main/resources`
  - `src/test/resources`

- File resources access:
  - General:
```java
ClassLoader classLoader = getClass().getClassLoader();
URL resourceUrl = classLoader.getResource("myfolder/myresource.txt");
```  
  - Spring framework:
```
Resource resource = new ClassPathResource("myfolder/myresource.txt");
```

- Target file access:
  - General:
```java
ClassLoader classLoader = getClass().getClassLoader();
URL resourceUrl = classLoader.getResource("myfolder/myresource.txt");
```  
  - Spring framework:
```
FileSystemResourceLoader resourceLoader = new FileSystemResourceLoader();
```

- `Equals and hashcode` come always together (comparison in collection with hash...)

## MAVEN

- Maven plugin for unit tests (UT) : `surefire`
- Maven plugin for integration tests (IT) : `failsafe`

## ERRORS

- Error: `Unsupported class file majir version 61` -> `JDK version not compatible`


## TOOLS

- Git do not default see Uppercase/lowercase changes by default ⚠️
