## Core kit setup
Please read core kit SDK setup part first. [ZTCoreKit](https://github.com/zhortech/ztcorekit-android-sdk/blob/main/README.md)

### Gradle

If you use Gradle to build your project — as a Gradle project implementation dependency:
```groovy
def zhortechSdkVersion = '1.0.52'
implementation "fr.zhortech.android:ztwarmkit:$zhortechSdkVersion-prod"
```

## Heating

To control heating use `ZTWarm` functions.\
`ZTWarm.startHeating(30)` will set target temperature in celsius and start heating.\
To stop heating use `ZTWarm.stopHeating()` \
`ZTWarm.getTargetTemperature()` will return current target temperature, if target temperature is 0 that means heating is disabled.
### Stop timer

You can set how long heating will work by starting timer `ZTWarm.startTimer(10)`, after timer finish heating will stop.\
`ZTWarm.stopTimer()` will stop timer if he in progress.
`ZTWarm.getRemainingTimer()` return remaining timer seconds

