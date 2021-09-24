# Python Cheat Sheet
####### Basic control flow, commands, in-build DS and more

# Basics

### Variables
| Syntax | Description |
| ------- | ----------- |
| `x=0, _x=0, X=0, s123 = 123` | All three are legal and different types of interger variables|
| `123s = 123` | illegal variable, error |
| `type(variable_name)` | gives type of the variable |

### Data Types
| Syntax | Description |
| ------- | ----------- |
| `x = 0, x = int(), ` | int declaration, int is same as long in #3.9 version|
| `y = 123.0, y = float(123)` | float declaration| |
| `` | double declaration|

### Boolean operations
|`x or y` | if x is false, then y, else x |
|`x and y` | if x is false, then x, else y |
|`not x` | if x is false, then True, else False |

### Comparisions
|`<` | strictly less than |
|`<=` | less than or equal |
|`>` | strictly greater than |
|`>=` | greater than or equal |
|`==` | equal |
|`!=` | not equal |
|`is` | object identity |
|`is not` | negated object identity |
|`in`| membership test, belongs to|
|`not in` | membership test, does not belong to|

### Arithematic operations on numeric types(int, float, complex)
| Syntax | Description |
| ------- | ----------- |
|`x + y` | sum of x and y |
|`x - y` | difference of x and y |
|`x * y` | product of x and y |
|`x / y` | quotient of x and y |
|`x // y` | floored quotient of x and y |
|`x % y` | remainder of `x / y` |
|`-x` | x negated |
|`+x` | x unchanged |
|`abs(x)` | absolute value or magnitude of x | 
|`int(x)` | x converted to integer |
|`float(x)` | x converted to floating point |
|`complex(re, im)` | a complex number with real part re, imaginary part im. im defaults to zero. |
|`c.conjugate()` | conjugate of the complex number c |
|`divmod(x, y)` | the pair (`x // y, x % y`) |
|`pow(x, y)`|x to the power y |
|`x ** y` | x to the power y |

### Sequence types - List, tuple, range
| Syntax | Description |
| ------- | ----------- |
|`x in s` | True if an item of s is equal to x, else False|
|`x not in s` |	False if an item of s is equal to x, else True|
|`s + t` |	the concatenation of s and t|
|`s * n or n * s`|	equivalent to adding s to itself n times|
|`s[i]` | ith item of s, origin 0|
|`s[i:j]` | slice of s from i to j|
|`s[i:j:k]` | slice of s from i to j with step k|
|`len(s)` | length of s|
|`min(s)` | smallest item of s|
|`max(s)` | largest item of s|
|`s.index(x[, i[, j]])` | index of the first occurrence of x in s (at or after index i and before index j)|
|`s.count(x)` | total number of occurrences of x in s|

### Mutable Sequence Types
| Syntax | Description |
| ------- | ----------- |
|`s[i] = x` | item i of s is replaced by x |
|`s[i:j] = t`	| slice of s from i to j is replaced by the contents of the iterable t |
|`del s[i:j]`	| same as `s[i:j] = []` |
|`s[i:j:k] = t`	| the elements of `s[i:j:k]` are replaced by those of t |
|`del s[i:j:k]`	| removes the elements of `s[i:j:k]` from the list |
|`s.append(x)`	| appends x to the end of the sequence (same as `s[len(s):len(s)] = [x]`) |
|`s.clear()`	| removes all items from s (same as `del s[:]`) |
|`s.copy()`	| creates a shallow copy of s (same as `s[:]`) |
|`s.extend(t)` or `s += t`	| extends s with the contents of t (for the most part the same as `s[len(s):len(s)] = t`) |
|`s *= n`	| updates s with its contents repeated n times |
|`s.insert(i, x)`	| inserts x into s at the index given by i (same as `s[i:i] = [x]`) |
|`s.pop()` or `s.pop(i)`	| retrieves the item at i and also removes it from s |
|`s.remove(x)`	| remove the first item from s where `s[i]` is equal to x |
|`s.reverse()`	| reverses the items of s in place |


### Numerical fucntions/operations
| Syntax | Description |
| ------- | ----------- |
|`math.trunc(x)`| x truncated to Integral |
|`round(x[, n])`| x rounded to n digits, rounding half to even. If n is omitted, it defaults to 0. |
|`math.floor(x)`| the greatest Integral <= x | 
|`math.ceil(x)`| the least Integral >= x |

### Bitwise Operations on Integer Types
| Syntax | Description |
| ------- | ----------- |
|`x | y`| bitwise or of x and y |
|`x ^ y`| bitwise exclusive or of x and y |
|`x & y`| bitwise and of x and y |
|`x << n`| x shifted left by n bits |
|`x >> n`| x shifted right by n bits |
|`~x`| the bits of x inverted|

### Lambda
| Syntax | Description |
| ------- | ----------- |
|`lambda_expr ::=  "lambda" [parameter_list] ":" expression` | lambda declaration|

### Bodmas extended version | Operations precedence 
| Syntax | Description |
| ------- | ----------- |
|`(expressions...),` |
| `[expressions...], {key: value...}, {expressions...}`| Binding or parenthesized expression, list display, dictionary display, set display |
|`x[index], x[index:index], x(arguments...), x.attribute`| Subscription, slicing, call, attribute reference |
|`await x`| Await expression |
|`**`| Exponentiation |
|`+x, -x, ~x`| Positive, negative, bitwise NOT |
|`*, @, /, //, %`| Multiplication, matrix multiplication, division, floor division, remainder |
|`+, -` | Addition and subtraction |
|`<<, >>` | Shifts |
|`&` | Bitwise AND |
|`^`| Bitwise XOR |
|`|`| Bitwise OR |
|`in, not in, is, is not, <, <=, >, >=, !=, ==`| Comparisons, including membership tests and identity tests |
|`not x` | Boolean NOT |
|`and`| Boolean AND |
|`or`| Boolean OR |
|`if – else` |`Conditional expression|
|`lambda`| Lambda expression |
|`:=`| Assignment expression |

### Control statements

| Statement | Syntax |
| ------- | ----------- |




### Errors and Exceptions
| E&E | Description |
| ------- | ----------- |
|AssertionError| Raised when the assert statement fails.|
|AttributeError|	Raised on the attribute assignment or reference fails.|
|EOFError|	Raised when the input() function hits the end-of-file condition.|
|FloatingPointError|	Raised when a floating point operation fails.|
|GeneratorExit|	Raised when a generator's close() method is called.|
|ImportError|	Raised when the imported module is not found.|
|IndentationError|	Raised when there is an incorrect indentation.|
|IndexError|	Raised when the index of a sequence is out of range.|
|KeyboardInterrupt|	Raised when the user hits the interrupt key (Ctrl+c or delete).|
|KeyError|	Raised when a key is not found in a dictionary.|
|MemoryError|	Raised when an operation runs out of memory.|
|NameError|	Raised when a variable is not found in the local or global scope.|
|NotImplementedError|	Raised by abstract methods.|
|OSError|	Raised when a system operation causes a system-related error.|
|OverflowError|	Raised when the result of an arithmetic operation is too large to be represented.|
|ReferenceError|	Raised when a weak reference proxy is used to access a garbage collected referent.|
|RuntimeError|	Raised when an error does not fall under any other category.|
|StopIteration|	Raised by the next() function to indicate that there is no further item to be returned by the iterator.|
|SyntaxError|	Raised by the parser when a syntax error is encountered.|
|SystemError|	Raised when the interpreter detects internal error.|
|SystemExit|	Raised by the sys.exit() function.|
|TabError|	Raised when the indentation consists of inconsistent tabs and spaces.|
|TypeError|	Raised when a function or operation is applied to an object of an incorrect type.|
|UnboundLocalError|	Raised when a reference is made to a local variable in a function or method, but no value has been bound to that variable.|
|UnicodeDecodeError|	Raised when a Unicode-related error occurs during decoding.|
|UnicodeEncodeError|	Raised when a Unicode-related error occurs during encoding.|
|UnicodeError|	Raised when a Unicode-related encoding or decoding error occurs.|
|UnicodeTranslateError|	Raised when a Unicode-related error occurs during translation.|
|ValueError|	Raised when a function gets an argument of correct type but improper value.|
|ZeroDivisionError|	Raised when the second operand of a division or module operation is zero.|



### Dictionaries
Configuring user information, initializing and cloning repositories


### One Liners
| Syntax | Description |
| ------- | ----------- |
|` 0 "if" x=0 "else" 1`| if else |
|`"Hello" if foo() else "Goodbye"` | if else example2 |
|`expr1 if condition1 else expr2 if condition2 else expr`| if elif else but not suggested to use |
|`"neg" if b<0 else "pos" if b>0 else "zero"` | if elif else but not suggested to use |
|`[[1+x+y*rowCount for x in range(rowCount)] for y in range(columnCount)] \
`output: [[1, 2, 3], [4, 5, 6], [7, 8, 9]]' ` | matrix create one liner |
| strings|
