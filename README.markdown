
## Introduction to App bundle sample project

The sample contains several modules.

`app` -> Contains the base application which always will be installed on device.

The `MainActivity` class demonstrates how to use the API to load and launch features.

Each feature as some distinctly unique characteristics.

- `dynamicfeature/install` -> Feature include at app install time and can delete anytime.
- `dynamicfeature/demand` -> Feature to request and download on your app as needed.
- `dynamicfeature/condition` -> Conditionally delivered feature based on hardware, max sdk version etc
- `dynamicfeature/instant` -> Instant Feature without an URL route. Loaded using SplitInstall API

The `AndroidManifest` files in each feature show how to declare a feature module as part of a dynamic app. Any module with the instant attribute is instant enabled. In this sample these can be found in the `instant/` folder:
