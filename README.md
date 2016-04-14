# xcode-codesnippet
Some useful code snippets for Xcode.

# Installation
* Open Xcode user data directory.
```sh
open ~/Library/Developer/Xcode/UserData
```
* Copy the `CodeSnippets` directory from this repository to Xcode user data directory.
* Restart Xcode.

# Objective-C Code Snippets
**alertview** `UIAlertView`.
```objective-c
UIAlertView *alert = [[UIAlertView alloc] initWithTitle:@"Title" message:@"<message>" delegate:nil cancelButtonTitle:@"OK" otherButtonTitles:nil, nil];
[alert show];
```

**aprop** nonatomic, assign property.
```objective-c
@property (nonatomic, assign) <type> <name>;
```

**dfn** `#define`.
```objective-c
#define <macro> <value>
```

**ffor** for loop.
```objective-c
for (int i = 0; i < <length>; i++) {
  <statements>
}
```

**globalq** `dispatch_async` on global queue.
```objective-c
dispatch_async(dispatch_get_global_queue(DISPATCH_QUEUE_PRIORITY_DEFAULT, 0), ^{
  <code>
});
```

**handlenoti** notification handler.
```objective-c
- (void)<method>:(NSNotification *)notification {
  <code>
}
```

**iinit** object initializer.
```objective-c
- (instancetype)init {
    self = [super init];
    if (self) {
		    <code>
	  }
    return self;
}
```

**ipt** `#import`.
```objective-c
#import <header>
```

**lstr** `NSLocalizedString`.
```objective-c
NSLocalizedString(@"<key>", nil)
```

**mainq** `dispatch_async` on main queue.
```objective-c
dispatch_async(dispatch_get_main_queue(), ^{
  <code>
});
```

**mlcomment** multiline comments.
```objective-c
/**
 * <content>
 */
```

**nslf** `NSLog` with Format String.
```objective-c
NSLog(@"%@", <object>);
```

**pinterface** private interface implementation.
```objective-c
@interface <class> ()

@end
```

**pmark** `#pragma mark`.
```objective-c
#pragma mark -
#pragma mark <name>
```

**postnoti** post a notification.
```objective-c
[[NSNotificationCenter defaultCenter] postNotificationName:<name>; object:nil userInfo:<userInfo>];
```

**prop** nonatomic, strong property.
```objective-c
@property (nonatomic, strong) <type> <name>;
```

**raprop** nonatomic, assign, readonly property.
```objective-c
@property (nonatomic, assign, readonly) <type> <name>;
```

**regnoti** register a notification.
```objective-c
[[NSNotificationCenter defaultCenter] addObserver:self selector:@selector(<selector>) name:<name> object:nil];
```

**remnoti** remove a notification.
```objective-c
[[NSNotificationCenter defaultCenter] removeObserver:self name:<name> object:nil];
```

**rprop** nonatomic, strong, readonly property.
```objective-c
@property (nonatomic, strong, readonly) <type> <name>;
```

**sharedinstance** shared instance.
```objective-c
+ (instancetype)sharedInstance {
    static <type> *result = nil;
    static dispatch_once_t onceToken;
    dispatch_once(&onceToken, ^{
        result = [[<type> alloc] init];
    });
    return result;
}
```

**strf** `StringWithFormat`.
```objective-c
[NSString stringWithFormat:@"%@", <object>]
```
