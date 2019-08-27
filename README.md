# SquareReaderTest

Step 1.
cd SquareReaderTest 
yarn

Step 2.
Change the settings on gradle.properties
SQUARE_READER_SDK_APPLICATION_ID=YOUR_SQUARE_READER_APP_ID
SQUARE_READER_SDK_REPOSITORY_PASSWORD=YOUR_SQUARE_READER_REPOSITORY_PASSWORD

Step 3.
Install the foo on your device
react-native run-android --variant=fooRelease

Step 4.
Install the bar on your device
react-native run-android --variant=barRelease

You should see the error below:
FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':app:installBarRelease'.
> com.android.builder.testing.api.DeviceException: com.android.ddmlib.InstallException: INSTALL_FAILED_CONFLICTING_PROVIDER: Package couldn't be installed in /data/app/com.bar-WsoeWMu222ss_Fvv_UvP8Q==: Can't install because provider name com.squareup.sdk.reader.api.leak-sentry-installer (in package com.bar) is already used by com.foo
