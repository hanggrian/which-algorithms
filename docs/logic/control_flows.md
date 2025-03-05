## Conditional

### If-else

=== "Java"
    ```java
    if (firstCondition) {
        System.out.println("First");
    } else if (secondCondition) {
        System.out.println("Second");
    } else {
        System.out.println("Third");
    }

    boolean get() {
        return firstCondition
            ? firstValue
            : secondValue;
    }
    ```
=== "Groovy"
    ```groovy
    if (firstCondition) {
        println 'First'
    } else if (secondCondition) {
        println 'Second'
    } else {
        println 'Third'
    }

    def get() {
        return firstCondition
            ? firstValue
            : secondValue
    }
    ```
=== "Kotlin"
    ```kotlin
    if (firstCondition) {
        println("First")
    } else if (secondCondition) {
        println("Second")
    } else {
        println("Third")
    }

    fun get() = if (firstCondition) firstValue else secondValue
    ```
=== "Python"
    ```python
    if first_condition:
        print('First')
    elif second_condition:
        print('Second')
    else:
        print('Third')

    def get():
        return first_value if first_condition else second_value
    ```
=== "JavaScript"
    ```javascript
    if (firstCondition) {
        console.log('First');
    } else if (secondCondition) {
        console.log('Second');
    } else {
        console.log('Third');
    }

    function get() {
        return firstCondition
            ? firstValue
            : secondValue;
    }
    ```
=== "TypeScript"
    ```typescript
    if (firstCondition) {
        console.log('First');
    } else if (secondCondition) {
        console.log('Second');
    } else {
        console.log('Third');
    }

    function get() {
        return firstCondition
            ? firstValue
            : secondValue;
    }
    ```

### Switch-case

=== "Java"
    ```java
    switch (value) {
        case firstValue:
            System.out.println("First");
            break;
        case secondValue:
            System.out.println("Second");
            break;
        default:
            System.out.println("Third");
            break;
    }
    ```
=== "Groovy"
    ```groovy
    switch (value) {
        case firstValue:
            println 'First'
            break
        case secondValue:
            println 'Second'
            break
        default:
            println 'Third'
            break
    }
    ```
=== "Kotlin"
    ```kotlin
    when (value) {
        firstValue -> // ...
        secondValue -> // ...
        else -> {
            // ...
        }
    }

    fun get() =
        when (value) {
            firstValue -> // ...
            secondValue -> // ...
            else -> {
                // ...
            }
        }
    ```
=== "Python"
    ```python
    match value:
        case first_value:
            print('First')
        case second_value:
            print('Second')
        case _:
            print('Third')
    ```
=== "JavaScript"
    ```javascript
    switch (value) {
        case firstValue:
            console.log('First');
            break;
        case secondValue:
            console.log('Second');
            break;
        default:
            console.log('Third');
            break;
    }
    ```
=== "TypeScript"
    ```typescript
    switch (value) {
        case firstValue:
            console.log('First');
            break;
        case secondValue:
            console.log('Second');
            break;
        default:
            console.log('Third');
            break;
    }
    ```

## Loops

### For

=== "Java"
    ```java
    for (int i = 0; i < 10; i++) {
        System.out.println(i);
    }

    for (Object o : objects) {
        System.out.println(o);
    }
    ```
=== "Groovy"
    ```groovy
    for (i in 0..9) {
        println i
    }

    for (var o in objects) {
        println o
    }
    ```
=== "Kotlin"
    ```kotlin
    for (i in 0 until 10) {
        println(i)
    }

    for (o in objects) {
        println(o)
    }
    ```
=== "Python"
    ```python
    for i in range(10):
        print(i)

    for i, o in enumerate(objects):
        print(o)
    ```
=== "JavaScript"
    ```javascript
    for (let i = 0; i < 10; i++) {
        console.log(i);
    }

    for (const o of objects) {
        console.log(o);
    }
    ```
=== "TypeScript"
    ```typescript
    for (let i = 0; i < 10; i++) {
        console.log(i);
    }

    for (const o of objects) {
        console.log(o);
    }
    ```

### While

=== "Java"
    ```java
    while (condition) {
        System.out.println("Hello");
    }

    do {
        System.out.println("World");
    } while (condition);
    ```
=== "Groovy"
    ```groovy
    while (condition) {
        println 'Hello'
    }

    do {
        println 'World'
    } while (condition)
    ```
=== "Kotlin"
    ```kotlin
    while (condition) {
        println("Hello")
    }

    do {
        println("World")
    } while (condition)
    ```
=== "Python"
    ```python
    while condition:
        print('Hello')
    ```
=== "JavaScript"
    ```javascript
    while (condition) {
        console.log('Hello');
    }

    do {
        console.log('World');
    } while (condition);
    ```
=== "TypeScript"
    ```typescript
    while (condition) {
        console.log('Hello');
    }

    do {
        console.log('World');
    } while (condition);
    ```

## Try-catch

=== "Java"
    ```java
    try {
        throw new Exception("Oops");
    } catch (Exception e) {
        e.printStackTrace();
    } finally {
        // ...
    }
    ```
=== "Groovy"
    ```groovy
    try {
        throw new Exception('Oops')
    } catch (Exception e) {
        e.printStackTrace()
    } finally {
        // ...
    }
    ```
=== "Kotlin"
    ```kotlin
    try {
        error("Oops")
    } catch (e: Exception) {
        e.printStackTrace()
    } finally {
        // ...
    }
    ```
=== "Python"
    ```python
    try:
        raise Exception('Oops')
    except Exception as e:
        print(e)
    finally:
        # ...
    ```
=== "JavaScript"
    ```javascript
    try {
        throw new Error('Oops');
    } catch (e) {
        console.error(e);
    } finally {
        // ...
    }
    ```
=== "TypeScript"
    ```typescript
    try {
        throw new Error('Oops');
    } catch (e) {
        console.error(e);
    } finally {
        // ...
    }
    ```
