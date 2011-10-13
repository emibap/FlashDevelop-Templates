Instructions for DISTRIBUTING* your application:

1. Download and Install both Flex and AIR SDKs:
- http://opensource.adobe.com/wiki/display/flexsdk/Flex+SDK
- http://www.adobe.com/special/products/air/sdk/
- Extract both SDKs
- Merge your Flex SDK and the AIR SDK (copy AIR SDK into Flex SDK folder)
- Set the Flex SDK Path of your project to the merged Flex SDK folder. (Or set the global Flex SDK path to the merged Flex SDK folder)
  Note: If you configure the global SDK under tools -> Program Settings... -> AS3Context -> InstalledFlexSDKs, you will not need to edit the batch files in order to configure it.  

2. Creating certificates:
-------------------------

2.1 iOS devices:
- Download and create a provisioning and a .p12 certificate file
  instructions link: (http://download.macromedia.com/pub/labs/packagerforiphone/packagerforiphone_devguide.pdf)
- Name the files "iphone_dev.p12" and "iphone_dev.mobileprovision" and copy them to the 'certificates' directory.

2.2 Android devices:
- Edit GenerateCertificate_android.bat and change the path to Flex SDK
- Run GenerateCertificate_android.bat

3. Setting up the App descriptor file:
--------------------------------------

3.1 iOS devices:
- Edit the file application_iOS.xml

3.2 Android devices:
- Edit the file application_android.xml

4. Testing the application:
---------------------------

4.1 iOS devices:
- By default you can test an iOS App by pressing F5 as usual, be aware that the available APIs on your desktop differ from the device.
- You can also run TestApplication_iOS.bat (set the flex SDK first)

4.2 Android devices:
- Run TestApplication_android.bat or modify the custom command in flash develop to target application_android.xml instead of application_iOS.XML

5. Packaging the application:
-----------------------------

5.1 iOS devices:
- Edit PackageApplication_iOS.bat and change the path to Flex SDK,
- Run PackageApplication_iOS.bat, you will be prompted for the certificate password.
- The packaged application should appear in your project in the 'iOS' directory.

5.2 Android devices:
- Edit PackageApplication_android.bat and change the path to Flex SDK,
- Run PackageApplication_android.bat, you will be prompted for the certificate password.
- The packaged application should appear in your project in the 'android' directory.

