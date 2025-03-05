## Collections

=== "Java"
    ```java
    Object[] subArray = Arrays.copyOfRange(array, start, end);
    List<Object> subList = list.subList(start, end);
    ```
=== "Groovy"
    ```groovy
    var subArray = arrayOrList[start..<end]
    ```
=== "Kotlin"
    ```kotlin
    val subArray = array.sliceArray(start until end)
    val subList = list.subList(start, end)
    ```
=== "Python"
    ```python
    sub_array = array[start:end]
    ```
=== "JavaScript"
    ```javascript
    let subArray = array.slice(start, end);
    ```
=== "TypeScript"
    ```typescript
    let subArray: any[] = array.slice(start, end);
    ```

## String

=== "Java"
    ```java
    String subString = string.substring(start, end);

    String subStringBefore = string.substring(0, string.indexOf("World"));
    String subStringBeforeLast = string.substring(0, string.lastIndexOf("World"));

    String subStringAfter = string.substring(string.indexOf("Hello") + "Hello".length());
    String subStringAfterLast = string.substring(string.lastIndexOf("Hello") + "Hello".length());
    ```
=== "Groovy"
    ```groovy
    var subString = string[start..<end]

    var subStringBefore = string[0..<string.indexOf('World')]
    var subStringBeforeLast = string[0..<string.lastIndexOf('World')]

    var subStringAfter = string[string.indexOf('Hello') + 'Hello'.length()..-1]
    var subStringAfterLast = string[string.lastIndexOf('Hello') + 'Hello'.length()..-1]
    ```
=== "Kotlin"
    ```groovy
    val subString = string.substring(start, end)

    val subStringBefore = string.substringAfter("World")
    val subStringBeforeLast = string.substringBeforeLast("World")

    val subStringAfter = string.substringBefore("Hello")
    val subStringAfterLast = string.substringAfterLast("Hello")
    ```
=== "Python"
    ```python
    sub_string = string[start:end]

    sub_string_before = string[:string.index('World')]
    sub_string_before_last = string[:string.rindex('World')]

    sub_string_after = string[string.index('Hello') + len('Hello'):]
    sub_string_after_last = string[string.rindex('Hello') + len('Hello'):]
    ```
=== "JavaScript"
    ```javascript
    let subString = string.substring(start, end);

    let subStringBefore = string.substring(0, string.indexOf('World'));
    let subStringBeforeLast = string.substring(0, string.lastIndexOf('World'));

    let subStringAfter = string.substring(string.indexOf('Hello') + 'Hello'.length);
    let subStringAfterLast = string.substring(string.lastIndexOf('Hello') + 'Hello'.length);
    ```
=== "TypeScript"
    ```typescript
    let subString: string = string.substring(start, end);

    let subStringBefore: string = string.substring(0, string.indexOf('World'));
    let subStringBeforeLast: string = string.substring(0, string.lastIndexOf('World'));

    let subStringAfter: string = string.substring(string.indexOf('Hello') + 'Hello'.length);
    let subStringAfterLast: string = string.substring(string.lastIndexOf('Hello') + 'Hello'.length);
    ```
