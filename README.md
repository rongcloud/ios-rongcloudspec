# Overview
To distinguish from the public cloud SDK, starting from January 1, 2024, customer-customized versions will no longer be published on the CocoaPods official website. Instead, the corresponding customized versions will be released in a dedicated Git repository to ensure that customers can easily access and use these versions. The published customized versions will not be removed and will still be available for download on the CocoaPods official website.

# Get Start

To download the customized version of the SDK, you can install RongCloudIM using CocoaPods by simply adding the following line to your Podfile.

To add the GitHub or Gitee source in the Podfile：

```
# gitee source
source 'git@gitee.com:rongcloud/ios-rongcloudspec.git'

# or github source
# source 'git@github.com:rongcloud/ios-rongcloudspec.git'

target 'AppProject' do
  pod 'RongCloudIM/IMLib', 'x.y.z'           #IMLib
  pod 'RongCloudIM/IMKit', 'x.y.z'           #IMKit
  pod 'RongCloudIM/Sight', 'x.y.z'           #Sight（optional）
  pod 'RongCloudIM/RongSticker', 'x.y.z'     #Sticker（optional）
  pod 'RongCloudIM/ContactCard', 'x.y.z'     #ContactCard（optional）
  pod 'RongCloudIM/LocationKit', 'x.y.z'     #LocationKit（optional）
end
```

To update the pod version in the same way as using CocoaPods：

```
# update pod
pod repo update

# install
pod install
```



