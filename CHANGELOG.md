# Change Log

## [1.1.0](https://github.com/auth0/JWTDecode.swift/tree/1.1.0) (2016-08-17)

[Full Changelog](https://github.com/auth0/JWTDecode.swift/compare/1.0.0...1.1.0)

**Changed:**

- Rework how claims are decoded [\#35](https://github.com/auth0/JWTDecode.swift/pull/35) ([hzalaz](https://github.com/hzalaz))
- Add expired method to A0JWT [\#25](https://github.com/auth0/JWTDecode.swift/pull/25) ([wkoszek](https://github.com/wkoszek))
- Require only App Extension Safe API (in iOS) [\#20](https://github.com/auth0/JWTDecode.swift/pull/20) ([hzalaz](https://github.com/hzalaz))

**Added:**

- Swift 2.3 [\#34](https://github.com/auth0/JWTDecode.swift/pull/34) ([hzalaz](https://github.com/hzalaz))
- Return JWT string representation [\#19](https://github.com/auth0/JWTDecode.swift/pull/19) ([hzalaz](https://github.com/hzalaz))
- Add tvOS Support [\#33](https://github.com/auth0/JWTDecode.swift/pull/33) ([adolfo](https://github.com/adolfo))

**Deprecated:**

To provide a better experience while dealing with claims and converting their values to Swift types, we deprecated the following method to retrive JWT claims

```swift
public func claim<T>(name: String) -> T?
```

In favor of the following method to retrieve the claim

```swift
let claim = jwt.claim(name: "claim_name")
```

and then you can try converting it's value to the proper type like

```swift
if let email = claim.string {
    print("JWT had email \(email)")
}
```

The supported conversions are:

```swift
var string: String?
var integer: Int?
var double: Double?
var date: NSDate?
var array: [String]?
```

## [1.0.0](https://github.com/auth0/JWTDecode.swift/tree/1.0.0) (2015-09-16)

[Full Changelog](https://github.com/auth0/JWTDecode.swift/compare/0.3.2...1.0.0)

**Fixed bugs:**

- Can this target 8.0 instead of 8.3? [\#10](https://github.com/auth0/JWTDecode.swift/issues/10)

**Merged pull requests:**

- Swift 2.0 [\#12](https://github.com/auth0/JWTDecode.swift/pull/12) ([hzalaz](https://github.com/hzalaz))

## [0.3.2](https://github.com/auth0/JWTDecode.swift/tree/0.3.2) (2015-08-21)

[Full Changelog](https://github.com/auth0/JWTDecode.swift/compare/0.3.1...0.3.2)

## [0.3.1](https://github.com/auth0/JWTDecode.swift/tree/0.3.1) (2015-07-25)

[Full Changelog](https://github.com/auth0/JWTDecode.swift/compare/0.3.0...0.3.1)

**Closed issues:**

- Failing to install via carthage [\#6](https://github.com/auth0/JWTDecode.swift/issues/6)

**Merged pull requests:**

- Carthage with submodules [\#8](https://github.com/auth0/JWTDecode.swift/pull/8) ([hzalaz](https://github.com/hzalaz))

- Build test only when running tests [\#7](https://github.com/auth0/JWTDecode.swift/pull/7) ([hzalaz](https://github.com/hzalaz))

## [0.3.0](https://github.com/auth0/JWTDecode.swift/tree/0.3.0) (2015-06-26)

[Full Changelog](https://github.com/auth0/JWTDecode.swift/compare/0.2.2...0.3.0)

**Merged pull requests:**

- Migrate to Swift [\#5](https://github.com/auth0/JWTDecode.swift/pull/5) ([hzalaz](https://github.com/hzalaz))

## [0.2.2](https://github.com/auth0/JWTDecode.swift/tree/0.2.2) (2015-06-26)

[Full Changelog](https://github.com/auth0/JWTDecode.swift/compare/0.2.1...0.2.2)

**Closed issues:**

- Issue with time of expiration. [\#3](https://github.com/auth0/JWTDecode.swift/issues/3)

## [0.2.1](https://github.com/auth0/JWTDecode.swift/tree/0.2.1) (2014-10-17)

[Full Changelog](https://github.com/auth0/JWTDecode.swift/compare/0.2.0...0.2.1)

**Closed issues:**

- Invalid id\_token claims part. Failed to decode base64 [\#1](https://github.com/auth0/JWTDecode.swift/issues/1)

**Merged pull requests:**

- base64 decode issue [\#2](https://github.com/auth0/JWTDecode.swift/pull/2) ([hzalaz](https://github.com/hzalaz))

## [0.2.0](https://github.com/auth0/JWTDecode.swift/tree/0.2.0) (2014-10-03)

[Full Changelog](https://github.com/auth0/JWTDecode.swift/compare/0.1.0...0.2.0)

## [0.1.0](https://github.com/auth0/JWTDecode.swift/tree/0.1.0) (2014-10-01)



\* *This Change Log was automatically generated by [github_changelog_generator](https://github.com/skywinder/Github-Changelog-Generator)*
