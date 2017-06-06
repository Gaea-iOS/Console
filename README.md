# Console
A simple console logger for swift

# Install 

in your *Cartfile* (don't have? create one!), add bellow in a new line.

```ruby
github "Gaea-iOS/Console" 
```

and then run the command in terminal:

```ruby
carthage update --platform iOS Console
```
# Usage

### easy to use:
```swift
Console.log(.debug, message: "this is a debug message")
```


### five log level are defined:

```swift
public enum LogLevel: Int, CustomStringConvertible {
        case error = 0
        case warning = 1
        case info = 2
        case debug = 3
        case verbose = 4
        }
```
if you want only log *error* level message, you should set maxLevel to *error*:

```swift
Console.maxLevel = .debug
```

enojoy it!
