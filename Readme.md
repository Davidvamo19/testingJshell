# Repository for testing jshell

jshell> int n=68;
n ==> 68

jshell> byte b=127;
b ==> 127

jshell> char c= 'B';
c ==> 'B'

jshell> b=n;
|  Error:
|  incompatible types: possible lossy con
version from int to byte
|  b=n;
|    ^

jshell> C=n;
|  Error:
|  cannot find symbol
|    symbol:   variable C
|  C=n;
|  ^

### After errors fixed

jshell> /edit 8
b ==> 68

jshell> /edit 9
c ==> 'D'
