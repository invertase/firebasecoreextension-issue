## Reproduction of FirebaseCoreExtension issue

### Steps to reproduce

1. Clone project locally and open via Xcode by opening workspace.

2. Go to root of project and run `pod install`.

3. See `FirebaseCoreExtension` pod is available and no issue in importing via `AppDelegate.m` (view in Xcode).

4. Now comment out `Firebase/Storage` pod in the Podfile and repeat step 2.

5. See that the header is not available and it is now missing from Pods/ directory in Xcode.