<p align="center">
  <img src="https://i.imgur.com/irnKSr0.png" height="160" alt="Feelm" /><br/>
</p>

<p align="center">
 <img src="https://img.shields.io/pub/v/string_extensions?color=637d0d&style=for-the-badge" alt="Version" /> <img src="https://img.shields.io/github/languages/code-size/esentis/string_extensions?color=637d0d&style=for-the-badge&label=size" alt="Version" /></br>
 <img src="https://travis-ci.com/esentis/string_extensions.svg?branch=master" alt="Version" />
 <a href='https://coveralls.io/github/esentis/string_extensions?branch=master'><img src='https://coveralls.io/repos/github/esentis/string_extensions/badge.svg?branch=master' alt='Coverage Status' /></a>
</br>
</p>

---

## Current Methods

- **You can use `>, >=, <, <=` operators, to compare `String` lengths. Also `-` to subtract a text from a `String`**

```dart
String s1 = 'esentis';
String s2 = 'dev';
print(s1 > s2); // prints true
print(s1 >= s2); // prints true
print(s1 < s2); // prints false
print(s1 <= s2); // prints false
print(s1-'tis'); // prints 'esen'
```

- **isGuid**

```dart
String foo = '6d64-4396-8547-1ec1b86e081e'
bool isGuid = foo.isGuid; // returns false
```

- **isNull**

```dart
String foo;
bool isNull = foo.isNull; // returns true
```

- **isUrl**

```dart
String foo = 'esentis';
bool isUrl = foo.isUrl; // 'false';
```

- **isDate**

```dart
String foo = 'esentis';
bool isDate = foo.isDate; // 'false';
```

- **isMail**

```dart
String foo = 'esentis@esentis.com';
bool isMail = foo.isMail; // returns true
```

```dart
String foo = 'esentis@esentis'
bool isMail = foo.isMail; // returns false
```

- **isIpv4**

```dart
String foo = '192.168.1.14';
bool isIpv4 = foo.isIpv4; // returns true
```

```dart
String foo = '192.168.1.14.150.1225';
bool isIpv4 = foo.isIpv4; // returns false
```

- **isIpv6**

```dart
String foo = '2001:0db8:85a3:0000:0000:8a2e:0370:7334';
bool isIpv6 = foo.isIpv6; // returns true
```

```dart
String foo = '92.168.1.14';
bool isIpv6 = foo.isIpv6; // returns false
```

- **isNumber**

```dart
String foo = '44';
bool isNumber = foo.isNumber; // returns true
```

```dart
String foo = '92.168.1.14';
bool isNumber = foo.isNumber; // returns false
```

- **isIn()**

```dart
String foo = '6d64-4396-8547-1ec1b86e081e';
var iterable = ['fff','gasd'];
bool isIn = foo.isIn(iterable); // returns false
```

- **toArray**

```dart
String foo = 'abracadabra';
List<String> fooArray = foo.toArray; // returns '[a,b,r,a,c,a,d,a,b,r,a]'
```

- **toCamelCase**

```dart
String foo = 'Find max of array';
String camelCase = foo.toCamelCase // returns 'findMaxOfArray'
```

- **toTitleCase**

```dart
String foo = 'hello world';
String fooTitled = foo.toTitleCase; // returns 'Hello World'
```

- **toSlug**

```dart
String foo = 'hello world';
String fooSlug = foo.toSlug; // returns 'hello_world'
```

- **toNum()**

```dart
String foo = '5.5';
double fooNum = foo.toNum(); // returns 5.5

String foo2 = '5';
int fooNum2 = foo.toNum(); // returns 5

String foo3 = '5f';
var fooNum2 = foo.toNum(); // returns null
```

- **toInt()**

```dart
String foo = '5.6';
int fooInt = foo.toInt(); // returns  5

String foo2 = '5';
int fooNum2 = foo.toInt(); // returns 5

String foo3 = '5f';
var fooNum2 = foo.toInt(); // returns null
```

- **toDouble()**

```dart
String foo = '5';
double fooDouble = foo.toDouble(); // returns 5.0

String foo = '5.5';
double fooDouble = foo.toDouble(); // returns 5.5

String foo = '5f';
var fooDouble = foo.toDouble(); // returns null
```

- **onlyLatin**

```dart
String foo = '4*%^55/es4e5523nt1is';
String letters = foo.onlyLatin; // returns 'esentis';
```

- **onlyGreek**

```dart
String foo = '4*%^55/σοφί4e5523nt1isα';
String letters = foo.onlyLatin; // returns 'σοφία';
```

- **onlyNumbers**

```dart
String foo = '4*%^55/es4e5523nt1is';
String onyNumbers = foo.onlyNumbers; // returns '455455231'
```

- **readTime({int wordsPerMinute})**

```dart
String foo =  'Hello dear friend how you doing ?';
int readTime = foo.readTime(); // returns 3 seconds.
```

- **removeNumbers**

```dart
String foo = 'es4e5523nt1is';
String noNums = foo.removeNumbers; // returns 'esentis'
```

```dart
String foo = '1244e*s*4e*5523n*t*1i*s';
String noNums = foo.removeNumbers; // returns 'e*s*e*n*t*i*s'
```

- **countWords**

```dart
String foo = 'Hello dear friend how you doing ?';
int count = foo.countWords; // returns 6 words.
```

- **capitalize**

```dart
String foo = 'hAckErrR';
String cFoo = foo.capitalize; // returns 'Hackerrr'.
```

- **removeLetters**

```dart
String foo = 'es4e5523nt1is';
String noLetters = foo.removeLetters; // returns '455231'
```

```dart
String foo = '1244e*s*4e*5523n*t*1i*s';
String noLetters = foo.removeLetters;// returns '1244**4*5523**1*'
```

- **charOccurences**

```dart
String foo = 'esentis';
List occurences = foo.charOccurences; // returns '[{e:2},{i:1},{n:1},{s:2},]'
```

- **mostFrequent**

```dart
String foo = 'Hello World';
String mostFrequent = foo.mostFrequent; // returns 'l'
```

- **reverse**

```dart
String foo = 'Hello World';
String reversed = foo.reverse; // returns 'dlrow olleH'
```

- **first()**

```dart
String foo = 'hello world';
String firstChars = foo.first(); // returns 'h'
```

- **last()**

```dart
String foo = 'hello world';
String lastChars = foo.last(); // returns 'd'
```

- **replaceGreek**

```dart
 String foo = 'Αριστοτέλης';
 String fooReplaced = foo.replaceGreek; // returns 'aristotelis'
```

- **findPatterns({required String pattern})**

```dart
String foo = 'abracadabra';
String fooOccs = foo.findPattern(pattern:'abr'); // returns '[0, 7]'
```

- **stripHtml**

```dart
String html = '<script>Hacky hacky.</script> <p>Here is some text. <span class="bold">This is bold. </span></p>';
String stripped = foo.stripHtml; // returns 'Hacky hacky. Here is some text. This is bold.'
```

- **repeat(int x)**

```dart
String string = 'foo';
String stripped = foo.repeat(2); // returns 'foofoo'
```

- **squeeze(String x)**

```dart
String foo = 'foofoofoofoofoo';
String fooSqueezed = foo.squeeze('o'); // 'fofofofofo';
```

- **hasSameCharacters**

```dart
String foo1 = 'ttttttt';
bool hasSame1 = foo.hasSameCharacters; // true;

String foo = 'ttttttt12'
bool hasSame2 = foo.hasSameCharacters; // false;
```

- **shuffle**

```dart
String foo = 'esentis';
String fooSqueezed = foo.shuffle; // 'teienss';
```

- **getLevenshtein(String word)**

```dart
String foo = 'esentis';
int distance = foo.getLevenshtein('esen'); // '3';
```

- **charCount(String char)**

```dart
String foo = 'esentis';
int distance = foo.charCount('e'); // '2';
```

- **formatWithMask(String mask)**

```dart
String string = 'esentisgreece';
String mask = 'Hello ####### you are from ######';
String masked = string3.formatWithMask(mask); // returns 'Hello esentis you are from greece'
```

- **removeFirst(int n)**

```dart
String foo = 'esentis';
String newFoo = foo.removeFirst(3); // 'ntis';
```

- **removeLast(int n)**

```dart
String foo = 'esentis';
String newFoo = foo.removeLast(3); // 'esen';
```

- **maxChars(int n)**

```dart
String foo = 'esentis';
String newFoo = foo.maxChars(3); // 'esen';
```

- **reverseSlash(int direction)**

```dart
String foo1 = 'C:/Documents/user/test';
String revFoo1 = foo1.reverseSlash(0); // returns 'C:\Documents\user\test'

String foo2 = 'C:\\Documents\\user\\test';
String revFoo2 = foo1.reverseSlash(1); // returns 'C:/Documents/user/test'
```

- **charAt(int index)**

```dart
String foo1 = 'esentis';
String char1 = foo1.charAt(0); // returns 'e'
```

- **ifEmpty(Function act)**

```dart
String foo1 = '';
foo1.ifEmpty(()=>'string is empty');
```

- **ifNull(Function act)**

```dart
String foo1;
foo1.ifEmpty(()=>'string is null');
```

- **append(String suffix)**

```dart
String foo1 = 'Hello';
foo1.append(' World'); // returns 'Hello World'
```

- **prepend(String prefix)**

```dart
String foo1 = 'World';
foo1.prepend('Hello'); // returns 'Hello World'
```

- **toPriceAmount({String? currencySymbol})**

```dart
String? s2 = '123333333';
String formatted = s2.toPriceAmount(currencySymbol: '€'); // returns '123.333.333,00 €'
```

- **getDayFromDate({String locale})**

```dart
String date = '2021-10-23';
String day = date.getDayFromDate(); // returns 'Saturday'
String grDay = date.getDayFromDate(locale:'el'); // returns 'Σάββατο'
```

- **getMonthFromDate({String locale})**

```dart
String date = '2021-10-23';
String month = date.getMonthFromDate(); // returns 'Octomber'
String grMonth = date.getMonthFromDate(locale:'el'); // returns 'Οκτωμβρίου'
```

- **firstDayOfMonth({String locale})**

```dart
String date = '2021-10-23';
String day = date.firstDayOfMonth(); // returns 'Friday'
String grDay = date.firstDayOfMonth(locale:'el'); // returns 'Παρασκευή'
```

- **lastDayOfMonth({String locale})**

```dart
String date = '2021-10-23';
String day = date.lastDayOfMonth(); // returns 'Sunday'
String grDay = date.lastDayOfMonth(locale:'el'); // returns 'Κυριακή'
```

- **leftOf(String char)**

```dart
String t = 'peanutbutter';
String left = date.leftOf('butter'); // returns 'peanut'
```

- **rightOf(String char)**

```dart
String t = 'peanutbutter';
String left = date.rightOf('peanut'); // returns 'butter'
```

- **truncate(int maxChars)**

```dart
String t = 'esentis';
String small = t.truncate(4); // returns 'esen...'
```

- **truncateMiddle(int maxChars)**

```dart
String t = 'esentis';
String small = t.truncateMiddle(2); // returns 'e...n'
```

- **quote**

```dart
String t = 'esentis';
String quote = t.quote; // returns "esentis"
```

- **trimAll**

```dart
String t = '     is       this     reality      ?';
String quote = t.trimAll; // returns "is this reality ?"
```
