## Objects

### Classes

=== "Java"
    ```java
    class Class {
        Object member = new Object();
    }
    ```
=== "Groovy"
    ```groovy
    class Class {
        var member = new Object()
    }
    ```
=== "Kotlin"
    ```kotlin
    class Class {
        val member = Any()
    }

    object Object {
        const val member = 0
    }
    ```
=== "Python"
    ```py
    class Class:
        def __init__(self):
            self.member = object()
    ```
=== "JavaScript"
    ```javascript
    class Class {
        let member = {};
    }
    ```
=== "TypeScript"
    ```typescript
    class Class {
        let member: any = {};
    }
    ```

### Interfaces

=== "Java"
    ```java
    interface Interface {
        void method();
    }
    ```
=== "Groovy"
    ```groovy
    interface Interface {
        void method()
    }
    ```
=== "Kotlin"
    ```kotlin
    interface Interface {
        fun method()
    }
    ```
=== "Python"
    ```py
    from abc import *

    class Interface(ABC):
        @abstractmethod
        def method(self):
            pass
    ```

### Enumerations

=== "Java"
    ```java
    enum Enumeration {
        ONE, TWO, THREE
    }
    ```
=== "Groovy"
    ```groovy
    enum Enumeration {
        ONE, TWO, THREE
    }
    ```
=== "Kotlin"
    ```kotlin
    enum class Enumeration {
        ONE, TWO, THREE
    }
    ```
=== "Python"
    ```py
    from enum import *

    class Enumeration(Enum):
        ONE = 1
        TWO = 2
        THREE = 3
    ```

## Overriding

### Text representation

=== "Java"
    ```java
    class Class {
        @Override
        public String toString() {
            return "Hello";
        }
    }

    // usage
    String text = String.format("%s World", new Class());
    ```
=== "Groovy"
    ```groovy
    class Class {
        @Override
        String toString() { 'Hello' }
    }

    // usage
    var text = "${new Class()} World"
    ```
=== "Kotlin"
    ```kotlin
    class Class {
        override fun toString() = "Hello"
    }

    // usage
    val text = "${new Class()} World"
    ```
=== "Python"
    ```py
    class Class:
        def __str__(self):
            return 'Hello'

    # usage
    text = f'{Class()} World'
    ```
=== "JavaScript"
    ```javascript
    class Class {
        toString() {
            return 'Hello';
        }
    }

    // usage
    let text = `${new Class()} World`;
    ```
=== "TypeScript"
    ```typescript
    class Class {
        toString(): string {
            return 'Hello';
        }
    }

    // usage
    let text: string = `${new Class()} World`;
    ```

### Equality

=== "Java"
    ```java
    class Class {
        @Override
        public boolean equals(Object other) {
            return true;
        }

        @Override
        public int hashCode() {
            return 0;
        }
    }

    // usage
    boolean isEqual = new Class().equals(new Class());
    ```
=== "Groovy"
    ```groovy
    class Class {
        @Override
        boolean equals(Object other) { true }

        @Override
        int hashCode() { 0 }
    }

    // usage
    var isEqual = new Class().equals(new Class())
    ```
=== "Kotlin"
    ```kotlin
    class Class {
        override fun equals(other: Any) = true

        override fun hashCode() = 0
    }

    // usage
    val isEqual = Class() == Class()
    ```
=== "Python"
    ```py
    class Class:
        def __eq__(self, other):
            return True

        def __hash__(self):
            return 0

    # usage
    is_equal = Class() == Class()
    ```
=== "JavaScript"
    ```javascript
    class Class {
        equals(other) {
            return true;
        }

        hashCode() {
            return 0;
        }
    }

    // usage
    let isEqual = new Class().equals(new Class());
    ```
=== "TypeScript"
    ```typescript
    class Class {
        equals(other: any): boolean {
            return true;
        }

        hashCode(): number {
            return 0;
        }
    }

    // usage
    let isEqual: boolean = new Class().equals(new Class());
    ```

### Comparison

=== "Java"
    ```java
    class Class implements Comparable<Class> {
        int number = 0;

        @Override
        public int compareTo(Class other) {
            return Integer.compare(number, other.number);
        }
    }

    // usage
    boolean isLesser = new Class().compareTo(new Class()) < 0;
    boolean isGreater = new Class().compareTo(new Class()) > 0;
    ```
=== "Groovy"
    ```groovy
    class Class implements Comparable<Class> {
        int number = 0

        @Override
        int compareTo(Class other) { Integer.compare(number, other.number) }
    }

    // usage
    var isLesser = new Class().compareTo(new Class()) < 0
    var isGreater = new Class().compareTo(new Class()) > 0
    ```
=== "Kotlin"
    ```kotlin
    class Class : Comparable<Class> {
        var number = 0

        override fun compareTo(other: Class) = number.compareTo(other.number)
    }

    // usage
    val isLesser = Class() < Class()
    val isGreater = Class() > Class()
    ```
=== "Python"
    ```py
    class Class:
        def __init__(self):
            self.number = 0

        def __lt__(self, other):
            return self.number < other.number

        def __gt__(self, other):
            return self.number > other.number

    # usage
    is_lesser = Class() < Class()
    is_greater = Class() > Class()
    ```
=== "JavaScript"
    ```javascript
    class Class {
        number = 0;

        compareTo(other) {
            return this.number - other.number;
        }
    }

    // usage
    let isLesser = new Class().compareTo(new Class()) < 0;
    let isGreater = new Class().compareTo(new Class()) > 0;
    ```
=== "TypeScript"
    ```typescript
    class Class {
        number: number = 0;

        compareTo(other: Class): number {
            return this.number - other.number;
        }
    }

    // usage
    let isLesser: boolean = new Class().compareTo(new Class()) < 0;
    let isGreater: boolean = new Class().compareTo(new Class()) > 0;
    ```
