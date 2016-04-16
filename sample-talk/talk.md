# Removing Currying from Swift

* Frederik Lohner
* David Zhuzhunashvili
* Derek Holland
* Justin Olson

# What is Swift

* Swift is Apples new programming language, it allows you to program for all Apple platforms.
* iOS, OS X, tvOS, watchOS.
* First introduced 2014
* Open Source as of Dec 3 2015!!

# What are the goals of Swift?

* Easy to understand

```swift
func greetings(name: String) -> String {
    return "Greetings \(name)!"
}
```	

# Swift is fairly Pythonic in nature

```swift
for car in cars {
    print(car)
}

for (key, value) in someDictionary {
	print("Key: \(key) has value \(value).")
}
```	

# Where are Swift changes discussed

* 

# What are the format of Swift changes

* 

# What is Currying

* Break an operation down to multiple functions based on inputs

# Example
```swift
func curried(x: Int)(y: String) -> Float {
	return Float(x) + Float(y)!
}
```

# Example cont

* So this would break down to

```swift
func curried(x: Int) -> (String) -> Float {
    return {(y: String) -> Float in
      return Float(x) + Float(y)!
    }
}
```

# Why would we remove currying

* Often causes issues with other features of a language without any real benefit
* Causes ambiguous syntax




