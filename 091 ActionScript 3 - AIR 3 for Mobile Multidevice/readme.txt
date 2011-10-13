Instructions for DISTRIBUTING* your application:

1. Download and Install both Flex and AIR SDKs:
- http://opensource.adobe.com/wiki/display/flexsdk/Flex+SDK
- http://www.adobe.com/special/products/air/sdk/
- Extract both SDKs
- merge your Flex SDK and the AIR SDK (copy AIR SDK into Flex SDK folder)
- set the Flex SDK Path of your project to the merged Flex SDK folder.

2. Creating certificates:
- download and create a provisioning and a .p12 certificate file
- instructions link: (http://download.macromedia.com/pub/labs/packagerforiphone/packagerforiphone_devguide.pdf)
- name the files "iphone_dev.p12" and "iphone_dev.mobileprovision" and copy them to the 'certificates' directory.

3. Packaging the application:
- edit PackageApplication.bat and change the path to Flex SDK,
- run PackageApplication.bat, you will be prompted for the certificate password.
- the packaged application should appear in your project in the 'iphone' directory.

* to test your application from FlashDevelop, just press F5 as usual, be aware that the available APIs on your desktop differ from the iPhone.
