<p align="center">
<img src="https://github.com/Nivashininivie/Kotlin-Multiplatform-blog/blob/main/kmp_final.png" alt="Description" width="650" />
</p>

# Kotlin Multiplatform Unveiled: How It Stacks Up Against Hybrid App Frameworks 

Nearly all the online service providers now offers mobile applications, increasing the demand for efficient Mobile Apps development. Depending on the requirements, developers can choose between Native or Hybrid.

While native mobile applications offer platform-specific advantages, they often come with challenges such as inconsistent behavior across platforms, higher development costs, and time constraints. To address these issues, many hybrid app development frameworks have been introduced, leading to an ongoing debate about choosing the right cross-platform tool. Kotlin Multiplatform is one such tool, announced by Google at Google I/O 2019. Since then, it has seen significant improvements and enhancements. 

Additionally, at the latest Google I/O 2024, Kotlin Multiplatform was recommended for sharing business logic across mobile, web, server, and desktop platforms. Google's next move involves integrating KMP into Google Workspace, indicating that we can expect significant progress on this platform.

## How KMP is different from other frameworks available? 
Eventhough there are many cross-platform tools available, KMP enables to maintain the same code for different platforms while retaining the flexibility and benefits of native programming, allowing developers to choose the approach that best fits their specific needs. Following are the usecases provided by KMP:

- **Shared Complex Modules with Native UI -** This approach is ideal when you already have separate platform-based applications but to avoid inconsistencies between platforms, critical functionalities can be developed as a Kotlin module and utilized across the entire codebase
- **Complete KMP Module with Native UI -** This is suitable for maintaining a native look and feel while ensuring consistent functionality across all platforms. By using platform-specific code for the UI, optimal performance is achieved, resulting in a smooth user experience. However, keep in mind that this will also double the associated costs and time.
- **100% KMP Module with CMP UI [Entire Logic & UI] -** When you want to have control over the UI as well. Maintaining separate UI code for each platform can double the time spent on development and fixes. The UI can be implemented using [Compose Multiplatform](https://www.jetbrains.com/compose-multiplatform/ "Compose Multiplatform")

- **Flexibility in Architecture -** While Flutter and React Native are powerful frameworks for cross-platform mobile development, they do impose certain constraints regarding UI design and architecture that KMP does not, making it a compelling choice for developers seeking flexibility and efficiency across multiple platforms.
- **Server-Side Development -** KMP also offers a robust environment for server-side development utilizing the Ktor framework, while in other frameworks, you would typically need to use additional technologies.

## Essential Takeaways

### Prerequisites 

Before diving into the details,  it's essential to have a piece of knowledge on the below:

1. **Kotlin:** Whether developing shared logic or the entire app functionality, having knowledge of Kotlin is essential.

2. **Platform-Specific Knowledge:** If you choose to work with native UI, it’s crucial to be familiar with Jetpack Compose for Android and Swift for iOS.

3. **Compose Multiplatform:** If the project involves handling the UI with Kotlin Multiplatform, understanding Compose Multiplatform is important.

### Compose Multiplatform
Compose Multiplatform (CMP) is a declarative framework built on Kotlin Multiplatform and Jetpack Compose, enabling developers to create user interfaces for multiple platforms, including iOS, macOS, Windows, Linux, and web applications.

<p align="center">
<img src="https://github.com/Nivashininivie/Kotlin-Multiplatform-blog/blob/main/cmp.png" alt="cmp" width="650" />
</p>

#### Key Features

* State-Driven: The framework automatically re-renders the necessary parts of the UI when the state changes.   
* Simplified Code: With its declarative syntax, CMP reduces boilerplate code, making it more concise and easier to read.  

**How CMP Renders UI?**
- Android: Jetpack Compose with the native Android toolkit.
- iOS: UIKit 
- Desktop (Windows, macOS, Linux): Uses Skia via Skiko 
- Web: Uses HTML Canvas or the DOM via WebAssembly or JavaScript.   
Since CMP leverages native rendering systems, the UI components not only look but also behave like native applications, which is a significant advantage.    

#### Stability constraints

As of September 2024, the stability of CMP varies by platform:  
| Platform                                   | Stability Stage |
|--------------------------------------------|-----------------|
| iOS                                        | Beta      |
| Web                                        | Alpha     |
| Android & Desktop (macOS, Windows, Linux) | Stable          |

### KMP Wizard
Unlike other tools, KMP offers a separate wizard for creating KMP app where you are presented with an user interface which lets you to create your own customised hybrid application
This wizard also simplifies the app creation process with standard templates which helps you to create apps based on your needs in just a few secs 
<p align="center">
<img src="https://github.com/Nivashininivie/Kotlin-Multiplatform-blog/blob/main/kmp_wiz.png" alt="kmpw" width="650" />
</p>
For more details, refer to this link [KMP wizard](https://kmp.jetbrains.com/ "KMP wizard")

### Interesting Case Studies
Here are some major apps that use KMP under the hood:
1. Jetbrains Toolbox 
2. Netflix
3. Philips
4. McDonald's and more...

Check out their [official site](https://www.jetbrains.com/help/kotlin-multiplatform-dev/case-studies.html "official site") for more details on the case studies

### Is it Still Evolving???
- Steeper Learning Curve: If you are new to KMP, you should have a basic understanding of Kotlin, Compose UI, Swift [If Native UI is preferred], etc
- Library support: While KMP is growing, still some libraries are not fully optimized for multiplatform use
- Beta Features: Some KMP features, particularly for iOS and web, may still be in beta or alpha stages, which can lead to stability issues.
- Lesser community & documentation: The community and available documentation are still developing compared to more established frameworks, which may pose challenges for developers seeking support.

Taking everything into account, KMP will be a great choice, 
- If you want to provide stable functionality while still offering a native user experience, you can utilize complete KMP modules and retain the UI natively.
- If you want to integrate with existing projects while enabling teams to adopt shared code without completely overhauling their current codebases
- Or if you prefer to share only a portion of the logic while retaining the rest of the functionalities as is on their respective platforms.
  
  

