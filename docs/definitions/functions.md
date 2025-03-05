## Methods

=== "Java"
    ```java
    void method(Object param) {
        System.out.println(param);
    }
    ```
=== "Groovy"
    ```groovy
    def method(var param) { println param }

    def multilineMethod(var param) {
        println param
        println param
    }
    ```
=== "Kotlin"
    ```kotlin
    fun method(param: Any) = println(param)

    fun multilineMethod(param: Any) {
        println(param)
        println(param)
    }

    var Any.variableMethod
        get() = "Hello"
        set(value) {
            println(value)
            println(value)
        }
    ```
=== "Python"
    ```py
    def method(param):
        print(param)
    ```

### Static modifier

=== "Java"
    ```java
    static void method(Object param) {
        System.out.println(param);
    }
    ```
=== "Groovy"
    ```groovy
    static def method(var param) { println param }
    ```
=== "Kotlin"
    ```kotlin
    companion object {
        fun method(param: Any) = println(param)
    }
    ```
=== "Python"
    ```py
    from typing import *

    @staticmethod
    def method(param):
        print(param)
    ```

## Lambdas

Lambdas are higher-order functional types passed as arguments.

=== "Groovy"
    ```groovy
    Closure listener = { param -> println(param) }

    Closure multilineListener = { param ->
        println(param)
        println(param)
    }
    ```
=== "Kotlin"
    ```kotlin
    val listener: (Any) -> Unit = { e -> println(param) }

    val multilineListener: (Any) -> Unit = { param ->
        println(param)
        println(param)
    }
    ```

### SAM conversions

=== "Java"
    ```java
    interface Lambda {
        void call(Object param);
    }

    Lambda lambda = param -> System.out.println(param);
    Lambda multilineLambda = param -> {
        System.out.println(param);
        System.out.println(param);
    };
    ```
=== "Groovy"
    ```groovy
    interface Lambda {
        void call(var param)
    }

    Lambda lambda = { param -> println param }
    Lambda multilineLambda = { param ->
        println param
        println param
    }
    ```
=== "Kotlin"
    ```kotlin
    fun interface Lambda {
        fun call(param: Any)
    }

    val lambda = Lambda { param -> println(param) }
    val multilineLambda =
        Lambda { param ->
            println(param)
            println(param)
        }
    ```
