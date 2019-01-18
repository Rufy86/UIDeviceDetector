# UIDeviceDetector
An extension of UIDevice class to detect the device simply and fast.

<br>

# Identifiable Devices
- [x] Air Pods
- [x] All iPhone (2018 updated)
- [x] All iPad (2018 updated)
- [x] All Apple Watch (2018 updated)
- [x] All Apple TV (2018 updated)
- [x] All iPods
- [x] Car Play

# How to Use

## To Check The Type of Device
This method check only if a device is an iPhone or an iPad regardless of the model
```Swift
if UIDevice.current.deviceType?.isPhone {
    print("It's an iPhone")
}

if UIDevice.current.deviceType?.isIPad {
    print("It's an iPad")
}
```

## To Detect The Type of Device

```Swift
switch UIDevice.current.deviceType!{
    case .iPhone35:
        print("It's an 3,5 inch iPhone")
    case .iPhone40:
        print("It's an 4 inch iPhone")
}
```

## To Detect The Model of Device
```Swift

switch UIDevice.current.deviceModel! {
case .appleWatch:
    print("It's 1st gen Apple Watch")
case .appleTV4K:
    print("It's Apple TV 4K")
}
```
