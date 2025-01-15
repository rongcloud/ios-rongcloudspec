# Overview
A customized version is a version tailored to specific customers' needs. These versions typically include specific features or adjustments required by the customer to meet their particular business needs or use cases.

Starting from January 1, 2025, to distinguish them from public cloud SDK pods, some customized versions will no longer be released on the CocoaPods official website. Instead, these corresponding customized versions will be published in public Git repositories to ensure that customers can easily access and use these versions. Previously released customized versions will not be removed and can still be downloaded through the CocoaPods official website.

# Get Start

To download the customized version of the SDK, add the following GitHub or Gitee source to your Podfile:

Gitee source:

```
#SDK 源
source 'git@gitee.com:rongcloud/ios-rongcloudspec.git'

target 'AppProject' do
   #pod sdk
   pod 'RongCloudIM/IMLib', 'x.y.z'           #IMLib
   pod 'RongCloudIM/IMKit', 'x.y.z'           #IMKit
   ...
end
```

GitHub  source:

```
source 'git@github.com:rongcloud/ios-rongcloudspec.git'

target 'AppProject' do
   #pod sdk
   pod 'RongCloudIM/IMLib', 'x.y.z'           #IMLib
   pod 'RongCloudIM/IMKit', 'x.y.z'           #IMKit
   ...
end
```

The public cloud SDK and customized SDK versions have the same pod import names. The above example only lists some commonly used SDK pod imports. For more references, consider [the following pod imports for IMKit](https://docs.rongcloud.cn/ios-imkit/import) and [the following pod imports for IMLib](https://docs.rongcloud.cn/ios-imlib/import):

When switching between the public cloud SDK and the customized SDK:

The version numbers of the public cloud SDK and the customized SDK are different. When switching, apart from modifying the version number:

To switch from the public cloud SDK to the customized SDK, simply add the GitHub or Gitee source mentioned above at the top of the Podfile.

To switch from the customized SDK to the public cloud SDK, just remove the mentioned GitHub or Gitee source added at the top of the Podfile.

To update the pod version in the same way as using CocoaPods：

```
# update pod
pod repo update

# install
pod install
```



