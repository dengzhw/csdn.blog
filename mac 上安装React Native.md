```````````````````
安装React Native
``````````````````
#####配置环境要求:

OS X：目前只有OS X中能够安转使用iOS的开发环境，并且Xcode 也只能运行在Mac上。
最新版的Xcode开发工具：在Mac的App Store上下载就可以；
推荐使用Homebrew来安转node，watchman和flow；
使用命令行brew install node来安装node；
使用命令行brew install - - HEAD watchman来安装watchman。我们推荐安装watchman，否者你可能会需要一个node文件来监控开发中的bug。
使用命令行brew install flow,如果你要使用flow的话。
快速开始

1. 使用命令行npm install -g react-native-cli;
1. 使用命令行react0-native init AwesomeProject；
1. 使用命令行cd AwesomeProject。
1. 在创建的文件夹AWesomeProject中：

使用Xcode打开AWesomeProject.xcodeproj文件并运行项目；
用你常用的文件编辑器打开index.ios.js文件，选中几行修改下代码；
在Xcode中打开iOS模拟器，按下组合键Cmd＋R（两次）重新加载应用，来观察修改的效果。
恭喜你！你刚刚已经成功地修改并运行了你的第一个React Native应用。

在已有的iOS应用中集成React Native。
在一个已经存在的App中集成React Native的内容，需要先安装React Native。不同于之前的安装方式，需要通过CocoPods来安转。CocoPods是用于iOS/Mac开发的一个包管理工具。在下啊面的三种应用场景下，你可以考虑在项目使用CocoaPods。

你想要将第三方库（第三方库使用了CocoPods）整合到新创建的React Native项目中；
目前你的项目使用CocoaPods来管理依赖和库；
你想要将React Native框架添加到一个现有的项目中。
如果你还没有安装CocoaPods，运行下面这个来安装：

  sudo gem install cocoapods
注意，你需要提前安转Ruby来使用gem命令。
根据React Native官网最新的说明，它用io.js来取代了node.js。让我们按照官网的指导来进行io.js的安装和配置。如果之前安装过node.js，则先运行命令：

  brew unlink node
这样可以完成node的解绑。然后运行：

brew install iojs
brew link iojs - -force
进行io.js的安装和配置。
现在我们已经准备好使用CocoaPods了，使用CocoaPods来安装React Native吧。

进入到所见iOS应用的文件目录，建立一个文件，命名为Podfile。在使用CocoaPods安装React Native时，Podfile相当于一个配置文件，它告诉安装程序需要下载安装哪些内容。
在Podfile中添加如下的内容。
pod 'React'
pod 'React/RCTText'
然后在终端执行一下命令：

  pod install
至此，你已经成功安装了React Native。
