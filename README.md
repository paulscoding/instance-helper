# instance-helper
### Make an instance of a class who are not in Project Files like in internet or in another folder.

## How To:
Make an instance of a class from a `java.net.URL` object or a `java.io.File` object.

## Examples:
#### User Class:

```java
public class User {

    private String name;
    private int age;

    public User(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }
}
```
#### Main Class:

```java
import java.io.File;

public class Main {

    public static void main(String[] args) {
        final Object obj = newInstance(new File("C://Users/Papa/Desktop/"), "User", new Class[]{
                String.class, int.class
        }, "Paul", 15);
    }
}
```