# py4j
A chinese pinyin library for Java. Supports multi-pinyin chinese word and external extension dictionary.

## maven dependency
```
<dependency>
    <groupId>com.bytebeats</groupId>
    <artifactId>py4j</artifactId>
    <version>1.0-SNAPSHOT</version>
</dependency>
```

## Usage
### single char
```
Py4j py4j = new Py4j();

char ch = '冒';
String[] arr_py = py4j.getPinyin(ch);
System.out.println(Arrays.toString(arr_py));
```

### word
```
Py4j py4j = new Py4j();

String chinese = "便宜坊";
String py = py4j.getPinyin(chinese);
System.out.println(py);
```

### Tips
Py4j instances are Thread-safe so you can reuse them freely across multiple threads.
