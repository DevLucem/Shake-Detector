# SHAKE DETECTOR //todo add the badges
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