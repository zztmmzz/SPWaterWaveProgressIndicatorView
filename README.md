# SPWaterProgressIndicatorView
This is custom subclass of UIView, which indicates the progress of task in percent.

## What it looks like?
![Presentation](https://raw.githubusercontent.com/antonio081014/SPWaterWaveProgressIndicatorView/master/3.gif)
## Directory
- **SPWaterProgressIndicatorView_README.md**
- **SPWaterProgressIndicatorView.hm**
- **SPWaterProgressIndicatorView.swift**
- **WaterWaveDemo** project demostrates how to use this class in Objective-C Project.
- **WaterWaveDemo_Swift** project demostrates how to use this class in Swift Project.

## How to user it?
- Add SPWaterProgressIndicatorView.hm files to the project.
- There are two ways to use this class:
  - Specify a `UIView`'s class as SPWaterProgressIndicatorView in IB.
  - Using `alloc` | `initWithFrame:` (Objective-C) to create and initialize an instance, then add it to a `UIView`.
  - Using `UIView` | `init(frame: CGRect)` (Swift) to create and initialize an instance, then add it to a `UIView`.

__Objective-C__
```
- (void)viewDidLoad {
    [super viewDidLoad];
    self.waterView = [[SPWaterProgressIndicatorView alloc] initWithFrame:self.view.bounds];
    self.waterView.center = self.view.center;
    [self.view addSubview:self.waterView];
    
}
```

__Swift__
```
override func viewDidLoad() {
    super.viewDidLoad()
        
    self.wave = SPWaterProgressIndicatorView(frame: self.view.bounds)
    self.wave.center = self.view.center;
    self.view.addSubview(self.wave)        
}
```

## Version
1.0

## Reference & Thanks
- [Stefan Ceriu's SCSiriWaveformView on Github](https://github.com/stefanceriu/SCSiriWaveformView)
