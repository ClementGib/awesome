- classpath : included directories where find classes and packages
  - target/classes
  - target/test-classes
  - target/lib
  - target/dependency
  - src/main/resources
  - src/test/resources

- File resources access:
  - ```
    ClassLoader classLoader = getClass().getClassLoader();
URL resourceUrl = classLoader.getResource("myfolder/myresource.txt");```  
