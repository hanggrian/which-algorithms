## Primitives

### Numbers

=== "Java"
    ```java
    import java.math.*;

    int intNumber = 0;
    short shortNumber = 0;
    long longNumber = 0L;
    double doubleDecimal = 0.0;
    float floatDecimal = 0.0f;

    Integer boxedIntNumber = 0;
    Short boxedShortNumber = 0;
    Long boxedLongNumber = 0L;
    Double boxedDoubleDecimal = 0.0;
    Float boxedFloatDecimal = 0.0f;

    BigInteger bigNumber = BigInteger.valueOf(0);
    BigDecimal bigDecimal = BigDecimal.valueOf(0.0);
    ```
=== "Groovy"
    ```groovy
    var intNumber = 0
    short shortNumber = 0
    var longNumber = 0L

    var doubleDecimal = 0.0d
    var floatDecimal = 0.0f

    var bigNumber = 0.toBigInteger()
    var bigDecimal = 0.0.toBigDecimal()
    ```
=== "Kotlin"
    ```kotlin
    val intNumber = 0
    val shortNumber: Short = 0
    val longNumber = 0L

    val doubleDecimal = 0.0
    val floatDecimal = 0.0f

    val bigNumber = 0.toBigInteger()
    val bigDecimal = 0.0.toBigDecimal()
    ```
=== "Python"
    ```py
    from decimal import *

    number = 0

    decimal = 0.0

    big_decimal = Decimal(0.0)
    ```
=== "JavaScript"
    ```javascript
    let number = 0;

    let decimal = 0.0;

    let bigNumber = BigInt(0);
    ```
=== "TypeScript"
    ```typescript
    let number: number = 0;

    let decimal: number = 0.0;

    let bigNumber: bigint = 0n;
    ```

#### Text conversion

=== "Java"
    ```java
    import java.math.*;

    int intNumber = Integer.parseInt("0");
    short shortNumber = Short.parseShort("0");
    long longNumber = Long.parseLong("0");
    double doubleDecimal = Double.parseDouble("0.0");
    float floatDecimal = Float.parseFloat("0.0");

    Integer boxedIntNumber = Integer.valueOf("0");
    Short boxedShortNumber = Short.valueOf("0");
    Long boxedLongNumber = Long.valueOf("0");
    Double boxedDoubleDecimal = Double.valueOf("0.0");
    Float boxedFloatDecimal = Float.valueOf("0.0");

    BigInteger bigNumber = new BigInteger("0");
    BigDecimal bigDecimal = new BigDecimal("0.0");
    ```
=== "Groovy"
    ```groovy
    var intNumber = '0'.toInteger()
    var shortNumber = '0'.toShort()
    var longNumber = '0'.toLong()

    var doubleDecimal = Double.parseDouble('0.0')
    var floatDecimal = Float.parseFloat('0.0')

    var bigNumber = '0'.toBigInteger()
    var bigDecimal = '0.0'.toBigDecimal()
    ```
=== "Kotlin"
    ```kotlin
    val intNumber = "0".toInt()
    val shortNumber = "0".toShort()
    val longNumber = "0".toLong()

    val doubleDecimal = "0.0".toDouble()
    val floatDecimal = "0.0".toFloat()

    val bigNumber = "0".toBigInteger()
    val bigDecimal = "0.0".toBigDecimal()
    ```
=== "Python"
    ```py
    from decimal import *

    number = int('0')

    decimal = float('0.0')

    big_decimal = Decimal('0.0')
    ```
=== "JavaScript"
    ```javascript
    let number = parseInt('0');

    let decimal = parseFloat('0.0');

    let bigNumber = BigInt('0');
    ```
=== "TypeScript"
    ```typescript
    let number: number = parseInt('0');

    let decimal: number = parseFloat('0.0');

    let bigNumber: bigint = BigInt('0');
    ```

### Text

JS and TS support multiline strings, but can't strip indentation.

=== "Java"
    ```java
    char character = 'a';

    Character boxedCharacter = 'a';

    String string = "Hello";

    String multilineString =
        """
        Hello
        World
        """;
    ```
=== "Groovy"
    ```groovy
    char character = 'a'

    var string = 'Hello'

    var multilineString =
        '''
        Hello
        World
        '''.stripIndent().trim()
    ```
=== "Kotlin"
    ```kotlin
    val character = 'a'

    val string = "Hello"

    val multilineString =
        """
        Hello
        World
        """.trimIndent()
    ```
=== "Python"
    ```py
    from textwrap import *

    string = 'Hello'

    multiline_string = \
        dedent(
            '''
            Hello
            World
            ''',
        ).strip()
    ```
=== "JavaScript"
    ```javascript
    let string = 'Hello';
    ```
=== "TypeScript"
    ```typescript
    let string: string = 'Hello';
    ```

#### Interpolation

=== "Java"
    ```java
    String lastName = "Simpson";
    String interpolatedString = String.format("%s, %s", lastName, "Homer");
    ```
=== "Groovy"
    ```groovy
    var lastName = 'Simpson'
    var interpolatedString = "$lastName, ${'Homer'}"
    ```
=== "Kotlin"
    ```kotlin
    val lastName = "Simpson"
    val interpolatedString = "$lastName, ${"Homer"}"
    ```
=== "Python"
    ```py
    last_name = 'Simpson'
    interpolated_string = f'{last_name}, {'Homer'}'
    ```
=== "JavaScript"
    ```javascript
    let lastName = 'Simpson';
    let interpolatedString = `${lastName}, ${'Homer'}`;
    ```
=== "TypeScript"
    ```typescript
    let lastName: string = 'Simpson';
    let interpolatedString: string = `${lastName}, ${'Homer'}`;
    ```

## Collections

### Array

Without explicit type, Groovy arrays are translated into `List`.

=== "Java"
    ```java
    int[] intNumberArray = {1, 2, 3};
    short[] shortNumberArray = {1, 2, 3};
    long[] longNumberArray = {1L, 2L, 3L};
    double[] doubleDecimalArray = {1.0, 2.0, 3.0};
    float[] floatDecimalArray = {1.0f, 2.0f, 3.0f};
    char[] characterArray = {'a', 'b', 'c'};
    Object[] array = {new Object(), new Object(), new Object()};
    ```
=== "Groovy"
    ```groovy
    int[] intNumberArray = [1, 2, 3]
    short[] shortNumberArray = [1, 2, 3]
    long[] longNumberArray = [1L, 2L, 3L]
    double[] doubleDecimalArray = [1.0, 2.0, 3.0]
    float[] floatDecimalArray = [1.0f, 2.0f, 3.0f]
    char[] characterArray = ['a', 'b', 'c']
    Object[] array = [new Object(), new Object(), new Object()]
    ```
=== "Kotlin"
    ```kotlin
    val intNumberArray = intArrayOf(1, 2, 3)
    val shortNumberArray = shortArrayOf(1, 2, 3)
    val longNumberArray = longArrayOf(1L, 2L, 3L)
    val doubleDecimalArray = doubleArrayOf(1.0, 2.0, 3.0)
    val floatDecimalArray = floatArrayOf(1.0f, 2.0f, 3.0f)
    val characterArray = charArrayOf('a', 'b', 'c')
    val array = arrayOf(Any(), Any(), Any())
    ```
=== "Python"
    ```python
    from array import *

    int_number_array = array('i', [1, 2, 3])
    short_number_array = array('h', [1, 2, 3])
    long_number_array = array('q', [1, 2, 3])
    double_decimal_array = array('d', [1.0, 2.0, 3.0])
    float_decimal_array = array('f', [1.0, 2.0, 3.0])
    character_array = array('u', 'abc')
    array = [object(), object(), object()]
    ```
=== "JavaScript"
    ```javascript
    let number_array = [1, 2, 3];
    let array = [{}, {}, {}];
    ```
=== "TypeScript"
    ```typescript
    let number_array: number[] = [1, 2, 3];
    let array: object[] = [{}, {}, {}];
    ```

### Lists

=== "Java"
    ```java
    List<Object> singletonList = Collections.singletonList(new Object());

    List<Object> immutableList =
        Collections.unmodifiableList(
            Arrays.asList(
                new Object(),
                new Object(),
                new Object()
            )
        );

    List<Object> mutableList = new ArrayList<>();
    mutableList.add(new Object());
    mutableList.add(new Object());
    mutableList.add(new Object());
    ```
=== "Groovy"
    ```groovy
    var singletonList = Collections.singletonList(new Object())

    var immutableList = [
        new Object(),
        new Object(),
        new Object(),
    ].asImmutable()

    var mutableList = [
        new Object(),
        new Object(),
        new Object(),
    ]
    ```
=== "Kotlin"
    ```kotlin
    val singletonList = listOf<Object>(Any())

    val immutableList =
        listOf<Object>(
            Any(),
            Any(),
            Any(),
        )

    val mutableList =
        mutableListOf<Object>(
            Any(),
            Any(),
            Any(),
        )
    ```
=== "Python"
    ```python
    immutable_list = (
        object(),
        object(),
        object(),
    )

    mutable_list = [
        object(),
        object(),
        object(),
    ]
    ```

### Sets

=== "Java"
    ```java
    Set<Object> singletonList = Collections.singleton(new Object());

    Set<Object> immutableList =
        Collections.unmodifiableSet(
            new HashSet<>(
                Arrays.asList(
                    new Object(),
                    new Object(),
                    new Object()
                )
            )
        );

    Set<Object> mutableList = new HashSet<>();
    mutableList.add(new Object());
    mutableList.add(new Object());
    mutableList.add(new Object());
    ```
=== "Groovy"
    ```groovy
    var singletonList = Collections.singleton(new Object())

    var immutableList = [
        new Object(),
        new Object(),
        new Object(),
    ].toSet().asImutable()

    var mutableList = [
        new Object(),
        new Object(),
        new Object(),
    ].toSet()
    ```
=== "Kotlin"
    ```kotlin
    val singletonList = setOf(Any())

    val immutableList =
        setOf(
            Any(),
            Any(),
            Any(),
        )

    val mutableList =
        mutableSetOf(
            Any(),
            Any(),
            Any(),
        )
    ```
=== "Python"
    ```python
    immutable_set = \
        fronzenset({
            object(),
            object(),
            object(),
        })

    mutable_set = {
        object(),
        object(),
        object(),
    }
    ```

### Maps

=== "Java"
    ```java
    Map<Object, Object> singletonMap =
        Collections.singletonMap(
            new Object(),
            new Object()
        );

    Map<Object, Object> immutableMap = new HashMap<>();
    immutableMap.put(new Object(), new Object());
    immutableMap.put(new Object(), new Object());
    immutableMap.put(new Object(), new Object());
    immutableMap = Collections.unmodifiableMap(immutableMap);

    Map<Object, Object> mutableMap = new HashMap<>();
    mutableMap.put(new Object(), new Object());
    mutableMap.put(new Object(), new Object());
    mutableMap.put(new Object(), new Object());
    ```
=== "Groovy"
    ```groovy
    var singletonMap =
        Collections.singletonMap(
            new Object(),
            new Object(),
        )

    var mutableMap = [
        new Object(): new Object(),
        new Object(): new Object(),
        new Object(): new Object(),
    ].asImmutable()

    var immutableMap = [
        new Object(): new Object(),
        new Object(): new Object(),
        new Object(): new Object(),
    ]
    ```
=== "Kotlin"
    ```kotlin
    val singletonMap = mapOf(Any() to Any())

    val immutableMap =
        mapOf(
            Any() to Any(),
            Any() to Any(),
            Any() to Any(),
        )

    val mutableMap =
        mutableMapOf(
            Any() to Any(),
            Any() to Any(),
            Any() to Any(),
        )
    ```
=== "Python"
    ```python
    mutable_map = {
        object(): object(),
        object(): object(),
        object(): object(),
    }
    ```
