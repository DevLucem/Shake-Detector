# SHAKE DETECTOR [![Lucem](https://camo.githubusercontent.com/cfcaf3a99103d61f387761e5fc445d9ba0203b01/68747470733a2f2f7472617669732d63692e6f72672f6477796c2f657374612e7376673f6272616e63683d6d6173746572)](https://about.me/lucem-anb)[![](https://jitpack.io/v/Lucem-Anb/Shake-Detector.svg)](https://jitpack.io/#Lucem-Anb/Shake-Detector)
This is an easy to use shake detector library on android devices

usage is literally **4 lines** of code

### Implementation

Add jitpack to repository
```
allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}
```

Add the dependency
```
implementation 'com.github.Lucem-Anb:shake-detector:0.0.1'
```

### Usage

Create a new shake detector where you want

```
new ShakeDetector(this, new ShakeListener() {
            @Override
            public void onShake() {
                Log.d("shake", "############################# Shaking it");
            }
        });
```

### Other Methods

kill listener `stopListening()`

start listener `startListening()`

set intensity of the shake `setShakeThreshold(float)`

set time difference between two shakes `setMinTimeBetweenShakesMillisecs(int)`

# Latest Version : 0.0.1
