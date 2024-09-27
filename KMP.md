<p align="center">
<img src="https://github.com/Nivashininivie/Kotlin-Multiplatform-blog/blob/main/kmp_final.png" alt="Description" width="650" />
</p>

# Kotlin Multiplatform for Hybrid Apps Development? 

Nearly all the online service providers now offer mobile applications, thereby increasing the demand for efficient Mobile Apps development. Depending on the requirements, developers can choose between Native or Hybrid.

While Native Mobile Applications provide platform-specific advantages, it often comes with challenges such as inconsistent behavior across platforms, higher development costs, and time constraints. 

To address this, nowadays companies prefer hybrid app development. In Google I/O 2019, google announced the emerging of new technology Kotlin Multiplatform. From there till now, there was a significant improvement & enhancements added. Let's checkout how KMP stands from other cross platform tools in the following.

## How KMP is different from other frameworks available? 
Eventhough there are lots of cross-platform tools available, KMP lets us to maintain the same code for different platforms while retaining the flexibility and benefits of native programming, allowing developers to choose the approach that best fits their specific needs.

#### Major Usecases:


<table>
  <tr>
    <td style="border: 2px solid #ddd; border-radius: 10px; padding: 20px; margin: 10px; background-color: #f0f8ff; width: 30%; text-align: center;">
      <h2> 1</h2>
      <p> Shared Complex Modules with Native UI </p>
    </td>
    <td style="border: 2px solid #ddd; border-radius: 10px; padding: 20px; margin: 10px; background-color: #e6ffe6; width: 30%; text-align: center;">
      <h2> 2 </h2>
      <p> Complete KMP Module with Native UI </p>
    </td>
    <td style="border: 2px solid #ddd; border-radius: 10px; padding: 20px; margin: 10px; background-color: #fff0f5; width: 30%; text-align: center;">
      <h2> 3 </h2>
      <p> 100% KMP Module with CMP UI [Entire Logic & UI] </p>
    </td>
  </tr>
</table>



- Case 1 is ideal when you already have separate platform-based applications but to avoid inconsistencies between platforms, critical functionalities can be developed as a Kotlin module and utilized across the entire codebase
- Case 2 is suitable for maintaining a native look and feel while ensuring consistent functionality across all platforms. By using platform-specific code for the UI, optimal performance is achieved, resulting in a smooth user experience. However, keep in mind that this will also double the associated costs and time.
- Case 3 is ideal when you want to have control over the UI as well. Maintaining separate UI code for each platform can double the time spent on development and fixes. The UI can be implemented using [Compose Multiplatform](http://https://www.jetbrains.com/compose-multiplatform/ "Compose Multiplatform")

## KMP's Essential Takeaways

### Prerequisites 

Before diving into the details,  it's essential to have a clear understanding of the following prerequisites:

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
For more details, refer to this link [KMP wizard](http://https://kmp.jetbrains.com/ "KMP wizard")

### Interesting Case Studies
Here are some major apps that use KMP under the hood:
1. Jetbrains Toolbox 
2. Netflix
3. Philips
4. McDonald's and more...

Check out their [official site](http://https://www.jetbrains.com/help/kotlin-multiplatform-dev/case-studies.html "official site") for more details on the case studies

### Is it Still Evolving???
- Steeper Learning Curve: If you are new to KMP, you should have a basic understanding of Kotlin, Compose UI, Swift [If Native UI is preferred], etc
- Library support: While KMP is growing, still some libraries are not fully optimized for multiplatform use
- Beta Features: Some KMP features, particularly for iOS and web, may still be in beta or alpha stages, which can lead to stability issues.
- Lesser community & documentation: The community and available documentation are still developing compared to more established frameworks, which may pose challenges for developers seeking support.

While the three use cases provide significant flexibility in selecting KMP, it is still an evolving technology. Developers should be ready to navigate the associated challenges. Despite having a smaller community, KMP shows great promise for cross-platform development as the ecosystem continues to mature.



