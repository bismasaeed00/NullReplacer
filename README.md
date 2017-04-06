# NullReplacer
These classes are for replacing NSNull objects from Arrays and Dictionaries when parsing API responses.

## How To Install
Download these files and add in your project.

import like this in your project: 

```
#import "NSArray+NullReplacement.h"
#import "NSDictionary+NullReplacement.h"
```

### How to use:

```
NSDictionary *data=@{@"status":201,@"message":null};
data=[data dictionaryByReplacingNullsWithBlanks];
```
output will be
```
@{@"status":201,@"message":@""}

```
It will remove all Null objects and replace them with empty strings to avoid crashes in your app.
