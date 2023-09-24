# React Native

## getting started with react native

**Name three Core Components of React Native and describe what they do.**

- View: A container that supports layout with flexbox, style, some touch handling, and accessibility controls.

- TextInput: Allows the user to enter text.

- ScrollView: A generic scrolling container that can contain multiple components and views.

**What problem does React Native solve (why call it native)?**

- React Native enables developers to use the React framework along with native platform capabilities.

**What are the building blocks of a React Native app? How does that compare to a React app?**

- Core components and Native components.

## expo

**What solution does expo provide?**

Ease of Getting Started: With Expo, setting up a new React Native project is straightforward, removing much of the initial setup and configuration.

Over-the-Air Updates: This feature allows you to push updates to your app without going through the app store review process.

Expo SDK: Provides access to system functionality such as the camera, push notifications, and sensors in a consistent manner across both Android and iOS.

Expo Go (previously known as the Expo client): An app available on Android and iOS that lets developers load and test their apps without having to go through the native build process. This greatly accelerates the development process.

Build Service: Expo can build your app binaries (.apk for Android and .ipa for iOS) in the cloud, so you don’t need Xcode or Android Studio.

Managed and Bare Workflows: While Expo initially only supported a managed workflow (where Expo handles most of the complexities), it now also offers a "bare" workflow for those who want more customization and are willing to take on more of the native build processes.

**Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the ____ workflow.**

- managed

**What is the difference between React Native and Expo?**

- React Native provides the fundamental architecture and building blocks for building mobile apps, Expo offers a layer on top that simplifies many aspects of development, especially the initial setup, testing, and building processes. However, this convenience comes at the cost of some flexibility.

## expo snack

**Checkout this tool. What does snack allow you to do?**

- Expo Snack is an interactive development environment and playground for React Native apps.

## ejecting

**What does “eject” mean within the context of Expo?**

- "Ejecting" in the context of Expo refers to the process of transitioning your Expo-managed project into a "bare" React Native project. When you eject, you're essentially taking your app out of the Expo environment, which allows you to write custom native code and integrate with native modules directly. After ejecting, you're responsible for native builds, dependencies, and managing the native codebase.

**When should you not eject?**

You might choose not to eject in the following scenarios:

- Simplicity: One of the main advantages of staying within the Expo managed environment is its simplicity. If your app doesn't need custom native modules or specific native configurations, staying in the managed workflow can save you from a lot of complexity related to native development.

- No Native Experience: If your team doesn't have experience with native development (Objective-C, Swift for iOS, or Java, Kotlin for Android), then ejecting can introduce challenges that might be hard to tackle.

- Over-the-Air (OTA) Updates: One of the powerful features of Expo is its support for Over-the-Air updates, allowing you to update your app without going through the app store review process. Though it's possible to set up OTA updates in a bare workflow, it's more straightforward in the managed workflow.

- Build Services: Expo provides cloud build services that take care of compiling and building the app binaries for you. Once you eject, you'll be responsible for setting up and managing your build process for both iOS and Android.

- Rapid Prototyping: If you're building a prototype or an MVP where speed is crucial, and you want to iterate quickly, the managed workflow in Expo can be beneficial.

**Why might you choose to eject?**

There are several reasons you might choose to eject:

- Native Modules: If you need to use a specific React Native community module that isn't supported by Expo or if you want to write your own native code, you'll need to eject.

- Full Control: Ejecting gives you complete control over the native side of your project. This means you can tweak configurations, adjust build settings, or optimize performance at the native level.

- Specific Native Features: For some features or third-party SDK integrations that require deep native integration and aren't available in the Expo SDK, ejecting might be necessary.

- App Size: Apps built with Expo can be larger because the Expo SDK includes a variety of libraries, whether you use them or not. Ejecting can allow you to minimize the app's size by including only the libraries you need.

- Custom Build Configurations: If you need specific build configurations or need to integrate with certain CI/CD processes, ejecting provides the flexibility you might need.
