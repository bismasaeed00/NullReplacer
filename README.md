# NullReplacer
These classes are for replacing NSNull objects from Arrays and Dictionaries when parsing API responses.

Download these files and add in your project.  …
import like this in your project: 
#import "NSArray+NullReplacement.h"
#import "NSDictionary+NullReplacement.h"

How to use:
NSArray *data=[result valueForKey:@"data"];
data=[data arrayByReplacingNullsWithBlanks];

It will remove all Null objects and replace them with empty strings to avoid crashes in your app.
