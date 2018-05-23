---
title: Visual Studio 2017 15.7 Release Notes
description: 'Release notes for the latest features and improvements in Visual Studio 2017. Plan better, code together and ship faster with Visual Studio.'
keywords: 'visualstudio> [!IMPORTANT]'
author: reshmim
ms.author: reshmim
manager: sacalla
ms.date: 05/08/2018
ms.topic: 'release-article, localize'
ms.prod: vs-devops-alm
ms.technology: vs-devops-articles
ms.assetid: 148a989e-80fd-448c-819e-b2e936f4f63f
hide_comments: true
hideEdit: true
---
<a id="top"></a>

# <a name="img-srcmediavslogo4svg-altvisual-studio-icon-visual-studio-2017-version-157-release-notes"></a><img src="media/vs_logo4.svg" alt="Visual Studio Icon"> **Visual Studio 2017 version 15.7 Release Notes**

****

| <a href="https://developercommunity.visualstudio.com/topics/visual+studio+2017.html?sort=newest&topics=visual studio 2017" target="blank">Developer Community</a> 
| <a href="https://docs.microsoft.com/visualstudio/productinfo/vs2017-system-requirements-vs" target="blank">System Requirements</a> 
| <a href="https://docs.microsoft.com/visualstudio/productinfo/vs2017-compatibility-vs" target="blank">Compatibility</a> 
| <a href="https://docs.microsoft.com/visualstudio/productinfo/2017-redistribution-vs" target="blank">Distributable Code</a> 
| <a href="https://www.visualstudio.com/license-terms" target="blank">License Terms</a> 
| <a href="https://blogs.msdn.microsoft.com/developer-tools" target="blank">Blogs</a> 
| <a href="https://developercommunity.visualstudio.com/topics/Known+Issue+in%3A+Visual+Studio+2017+Version+15.7.html" target="blank">Known Issues</a> |

****

> [!NOTE]
> If you are accessing this page from a non-English language version, and want to see the most up-to-date content, please visit this Release Notes page in <a href="https://docs.microsoft.com/visualstudio/releasenotes/vs2017-relnotes" target="blank">English</a>. You can change the language of this page by clicking the <img src="media/globe7.png"></a> icon in the [page footer](#bottom) and selecting your desired language.

<hr style="border:1px solid Silver">

Click a button to download the latest version of Visual Studio 2017. For instructions on installing and updating Visual Studio 2017, see <a href="https://docs.microsoft.com/visualstudio/install/update-visual-studio" target="blank">Update Visual Studio 2017 to the most recent release</a>. Also, see instructions on <a href="https://docs.microsoft.com/visualstudio/install/create-an-offline-installation-of-visual-studio" target="blank">how to install offline</a>.

<a href="https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Community&rel=15" target="blank"><img src="media/Download_Community_2017.svg"></a>          <a href="https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Professional&rel=15" target="blank"><img src="media/Download_Professional_2017.svg"></a>          <a href="https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Enterprise&rel=15" target="blank"><img src="media/Download_Enterprise_2017.svg"></a>

****

## <a name="whats-new-in-157"></a>**What's New in 15.7**

**The Visual Studio Blog** is the official source of product insight from the Visual Studio Engineering Team. You can find in-depth information about the Visual Studio 15.7 releases in the following posts:
* <a href="https://aka.ms/build2018-vsideannounce" target="blank">Visual Studio 15.7 Minor Release</a> --  _Read the latest blog post!_
* <a href="https://blogs.msdn.microsoft.com/visualstudio/2018/04/09/visual-studio-2017-version-15-7-preview-3/" target="blank">Visual Studio 15.7 Preview 3</a>
* <a href="https://blogs.msdn.microsoft.com/visualstudio/2018/03/21/visual-studio-2017-version-15-7-preview-2/" target="blank">Visual Studio 15.7 Preview 2</a>
* <a href="https://blogs.msdn.microsoft.com/visualstudio/2018/03/13/visual-studio-2017-version-15-7-preview-1/" target="blank">Visual Studio 15.7 Preview 1</a>

### <a name="visual-studio-2017-version-157-releases"></a>Visual Studio 2017 version 15.7 Releases
* May 08, 2018 -- [Visual Studio 2017 version 15.7.1](#15.7.1) Servicing Update <img src="media/New_button_bg2.svg">
* May 07, 2018 -- [Visual Studio 2017 version 15.7.0](#15.7) Minor Release

### <a name="visual-studio-2017-version-157-announcements"></a>Visual Studio 2017 version 15.7 Announcements
* May 08, 2018 -- [Visual Studio 2017 version 15.7 Security Advisory](#15.7.S) Notice <img src="media/New_button_bg2.svg">

### <a name="summary-of-notable-new-features-in-157"></a>Summary of Notable New Features in 15.7
* We added support to change [installation locations](#install2).
* You can [Save All](#ide3) your pending changes before you start your update.
* The update dialog provides you even more details about your [update](#install) during installation.
* [C# 7.3](#csharp) is included in Visual Studio version 15.7.
* We improved solution [load time](#perf) for C# and VB projects.
* We made numerous updates to [F# and its tools](#fsharp), with a focus on performance.
* [We reduced the time](#perf) to enable IntelliSense for large .NET Core projects by 25%.
* We made Quick Info improvements and new [.NET refactorings](#dotnet_productivity) like convert `for`-to-`foreach` and make private fields `readonly`.
* We added the ability to [publish ASP.NET Core applications to App Service Linux without containers](#ASP.NET).
* Live Unit Testing works with [embedded pdbs](#test) and supports projects that use reference assemblies.
* The Test Explorer has more [responsive icons](#test) during test runs.
* C++ developers can use [CodeLens for unit testing](#C++P3).
* We added new rules enforcing items from the [C++ Core Guidelines](#C++P2). 
* Debugging large solutions with [/Debug:fastlink PDBs](#C++P1) is more robust.
* CMake integration supports [CMake 3.11 and static analysis](#C++P4).
* [Python](#Python) projects support type hints in IntelliSense, and a Run MyPy command has been added to look for typing errors in your code.
* Conda environments are supported in [Python](#Python) projects.
* We added a next version of our [Python](#Python) debugger based on the popular open source pydevd debugger.
* [TypeScript 2.8](#TypeScript-JavaScript) is included in Visual Studio version 15.7.
* We improved [Kestrel HTTPs support](#webtools) during debugging. 
* We added support for [JavaScript debugging with Microsoft Edge](#Edge).
* The Debugger supports VSTS and GitHub [Authentication for Source Link](#debug2).
* IntelliTrace’s [step-back debugging feature](#debug) is supported for debugging .NET Core projects. 
* We added IntelliTrace support for taking [snapshots](#debug3) on exceptions.
* We removed the blocking modal dialog from [branch checkouts in Git](#perf) when a solution or project reload is not required.
* You have the [option to choose between OpenSSL and SChannel in Git](#te).
* You can create and associate Azure Key Vaults from within the [Visual Studio IDE](#KeyVault).
* Visual Studio Tools for Xamarin can [automatically install missing Android API levels](#android-auto-sdk) required by Xamarin.Android projects.
* [The Xamarin.Forms XAML editor](#xaml) provides IntelliSense and quick fixes for conditional XAML.
* [Visual Studio Build Tools](#BuildTools) now supports installing into a container, and we added support for building Azure, UWP, and additional project types. 
* You can create build servers without [installing all of Visual Studio](#BuildToolsUWP).
* The [Windows 10 April 2018 Update SDK - Build 17134](#WinTools) is the default required SDK for the Universal Windows Platform development workload.
* We added support for [Visual State Management](#WinTools) for all UWP apps and more.
* We enabled automatic updates for [sideloaded APPX packages](#appinstaller).
* You have new tools for [migrating to NuGet PackageReference](#nugetpreview3).
* We added support for [NuGet package signatures](#NuGet).
* We added Service Fabric Tooling for the [6.2 Service Fabric release](#SFTools).
* We updated [Entity Framework Tools](#EFTools) to work with the EF 6.2 runtime and to improve reverse engineering of existing databases.


<hr style="border:1px solid red">

## <a name="top-issues-fixed-in-157"></a>**Top Issues Fixed in 15.7**
These are the customer-reported issues addressed in 15.7: 
* <a href="https://developercommunity.visualstudio.com/content/problem/208727/mfc-class-wizard-cant-add-control-member-variables.html" target="blank">MFC Class Wizard can't add control member variables</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/65159/test-explorer-intermittently-never-finishes-findin.html" target="blank">Test Explorer intermittently never finishes finding tests</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/161935/internal-compiler-error-in-vs155.html" target="blank">Internal compiler error in VS15.5</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/25594/visual-studio-build-tools-2017-is-missing-msbuild.html" target="blank">Visual Studio Build Tools is missing MSBuild Web SDKs</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/31149/vs2017-deployed-git-doesnt-support-self-signed-cer.html" target="blank">VS2017 deployed Git doesn't support self-signed certs</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/212073/visual-studio-hang-during-nuget-package-update.html" target="blank">Visual Studio hangs during NuGet package update</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/203619/visual-studio-installer-showing-unsupported-comman.html" target="blank">Visual Studio Installer shows "unsupported command" after update</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/160918/waiting-for-microsoftvisualstudiographicsenabletoo.html" target="blank">Visual Studio installation hangs at "Waiting for Microsoft.VisualStudio.Graphics.EnableTools"</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/134264/visual-states-not-exist-in-vs-blend-2017-for-proje.html" target="blank"> XAML designer doesn't recognize Visual State, throws "Windows 10 Fall Creators Update (10.0; Build 16299)" error</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/169910/razor-cshtml-bad-automatic-formatting.html" target="blank">The automatic formatting in Razor (cshtml)  breaks on paste</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/183705/no-diagnostic-on-invalid-member-initialization-sin.html" target="blank">No diagnostic on invalid member initialization since MSVC 14.12</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/192062/static-resource-defined-in-themedictionaries-not-f.html" target="blank">Static resource defined in ThemeDictionaries not fetched while edit a copied template for custom control</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/192168/add-new-file-online-template-basename-empty-string.html" target="blank">Add New File -> Online Template "baseName empty string" generates Non-Fatal Error</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/31256/microsoftalmsharedremotingremotecontainerdll-high.html" target="blank">Microsoft.Alm.Shared.Remoting.RemoteContainer.dll generates high CPU usage</a>.
* <a href="https://developercommunity.visualstudio.com/content/problem/155117/razor-cshtml-helper-formatting-incorrect.html" target="blank">Razor cshtml helper format is not done incorrectly</a>.

See all customer-reported issues fixed in Visual Studio 2017 version 15.7.

<a href="https://developercommunity.visualstudio.com/topics/fixed+in%3A+visual+studio+2017+version+15.7.html" target="blank"><img src="media/DevComm_button_sm2.svg" alt="The Developer Community Portal"></a>

****

## <a name="details-of-whats-new-in-157"></a>**Details of What's New in 15.7**

## <img src="media/News_icon.svg" alt="Release Notes Icon"> <a id="15.7"></a>Visual Studio 2017 version 15.7.0
_released on May 07, 2018_

### <a name="new-features-in-157"></a>**New Features in 15.7**
### <a id="perf"></a>Performance
* In this release, we improved solution load time for C# and VB projects by an average of 20%.
* In large .NET Core projects, we reduced the time to load IntelliSense by 25%.
* When switching branches in Git, the modal progress dialog has been removed when solutions and projects do not need to be reloaded.

### <a id="install"></a>Installing Visual Studio
* The update dialog provides more details about your update, such as what's new, the download size, and the latest update version.
* **Improved save experience:**<a id="ide3"></a> Before you update Visual Studio, all pending changes will be saved locally _first_ -- before starting the update. The update dialog, will show a **Save All & Update** button instead of **Update Now**. 
* We reduced the installation footprint on the system drive by moving the download cache, shared components, some SDKs, and tools to different drives _(Figure 1)_.

<figure><center><img src="media/InstallLocations-2.png" alt="Install Locations"><figcaption><em>(Figure 1) Choose install locations</em></figcaption></center></figure>

<a id="install2"></a>There are three locations you can manage, and these locations can only be set with your very **first installation**: * **Visual Studio core product:** This location is for files that are specific to the version of Visual Studio you selected to install. 
  * **Download cache:** Installation files and manifests will be downloaded to this location. If you decide not to keep the download cache by unchecking the check box, the files will be removed after installation completes.
  * **Shared components, tools, and SDKs:** This location is for files that are shared by side-by-side Visual Studio installations.
  > [!NOTE] Tools and SDKs that have different rules as to where they are installed, won’t be installed to this drive. The tool/SDK specific rules take precedence.
  
  > [!NOTE]
  > Users can disable the package cache and set the location. 

### <a id="ide"></a>Visual Studio IDE

The dialog window *(Figure 2)* that indicates which long running operation is keeping Visual Studio busy, is now screen reader accessible (for example, NVDA, Narrator, etc.). When the dialog is shown by Visual Studio, the screen reader plays an audio cue indicating new information is visible on the screen. Users can read the contents of the dialog or interact with the **Cancel** button when available by invoking the **Change View** command in Narrator.

<figure><center><img src="media/TWD.png" alt="Wait dialog"><figcaption><em>(Figure 2) Loading dialog window, now screen reader accessible</em></figcaption></center></figure>

  > [!NOTE] 
  > For full Narrator support, you must be using Windows 10 Redstone 4 (RS4) builds.

### <a name="visual-c-improvements"></a>Visual C++ Improvements
* This release contains a fix for a local information disclosure vulnerability in PDB files as described in [CVE-2018-1037](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2018-1037).
* [C5045](https://blogs.msdn.microsoft.com/vcblog/2018/04/20/spectre-diagnostic-in-visual-studio-2017-version-15-7-preview-4/) is a new compiler diagnostic that lets you see code patterns where the compiler would have inserted a Spectre mitigation.
* Visual Studio's bundled CMake installation has been upgraded from 3.10 to 3.11.<a id="C++P4"></a>
* CMake projects support static analysis of C++ code, such as VCXProj. 
* MSVC supports the C++17 feature [P0426R1](https://wg21.link/p0426r1) "constexpr for std::char_traits," which makes `std::string_view much` more usable at compile time.
* Use [CodeLens above each of your unit tests](https://aka.ms/codelensUT) to Run, Debug, and view Test Status<a id="C++P3"></a> _(Figure 3)_.
<figure><center><img src="media/UnitTest.png" alt="Use CodeLens above each of your unit tests"><figcaption><em>(Figure 3) Use CodeLens above each of your unit tests</em></figcaption></center></figure>

* We updated the Visual Studio iOS development tools for C++ to work with Xcode 9.
* We added /analyze:ruleset option to cl.exe for filtering down warnings in the C++ Code Analysis tools based on ruleset configuration. This results in a consistent experience between standalone invocations of the compiler and the IDE and improves performance by running only the rules mentioned in ruleset.
* Inheriting a constructor now works the same as inheriting any other base class member. Previously, this worked by declaring a new constructor that delegates to the original; with this change, base class constructors are visible in a derived class as if they were derived class constructors, improving consistency in C++.
* Templates that are designed to take any type as a non-type parameter can now use the `auto` keyword in the template parameter list. This allows instantiations to use any type instead of needing to determine and supply the type of template parameter at the point of instantiation.
* `std::launder` is now supported.
* Two-phase name lookup operates correctly in almost all cases. Some edge cases, such as non-dependent function calls to overloaded operators, will be fixed in a future update.
* The MSVC compiler toolset conforms with the C++ 17 Standard. When compiling with the /Zc:__cplusplus switch, the value of the __cplusplus macro reflects the correct Standard version numbers.
* The Visual C++ Runtime supports mitigations for the Spectre variant 1 vulnerability. The toolset includes mitigated and non-mitigated versions of the DLLs. Enabling the Spectre Mitigation feature in the Code Generation property page will also cause linking to the mitigated version of the DLL. [More information about Spectre mitigations](https://blogs.msdn.microsoft.com/vcblog/2018/01/15/spectre-mitigations-in-msvc) is available on the Visual C++ Team Blog. 
* Enabled compiler support for [Spectre mitigations](https://blogs.msdn.microsoft.com/vcblog/2018/01/15/spectre-mitigations-in-msvc/) in non-optimized builds (/Od).
* The /Zf switch is now enabled by default, which enables faster PDB generation when using multiple compilation processes.
* We significantly improved the code generation for /await. We re-implemented coroutines in the code generator to improve reliability, fixing the vast majority of bugs.
* The [CMake Targets View](https://aka.ms/cmaketargetsview) provides an alternative way to view a CMake project's source in the Solution Explorer; instead of a folder-based view, it organizes the code into individual CMake targets _(Figure 4)_. The organization is similar to the organization of the Project and Solution files created by the CMake "Visual Studio" generator.
<figure><center><img src="media/Cmake.png" alt="CMake Targets View"><figcaption><em>(Figure 4) CMake Targets View</em></figcaption></center></figure>

* Source files (.cpp) belonging to CMake projects can be built individually via the CMake menu or by right-clicking on a source file in the Solution Explorer.
* Unknown macros that cause tag-parsing errors are now underlined with green squiggles. A quick action is available to automatically add the macro to a C++ Hint file to resolve the issue. All tag-parsing errors in the Solution or folder can be listed by clicking **Display Tag Parser Errors** on the Project menu.
* Add headers to the CppProperties.json include path with quick actions in Open Folder.
* Headers from Linux and Unix-like systems are now automatically downloaded for use by IntelliSense on Windows. These are also used to provide an enhanced IntelliSense experience for Linux native Platform development.
* We added five new rules enforcing items from the<a id="C++P2"></a> [C++ Core Guidelines](https://github.com/isocpp/CppCoreGuidelines) regarding use of the [Guidelines Support Library](https://github.com/Microsoft/GSL).
* We allow public base classes in aggregate types, so that they can be initialized using aggregate initialization syntax without writing boilerplate constructors. In the braced initializer list, bases are initialized first, followed by data members.
* Extend [template argument deduction](http://www.open-std.org/jtc1/sc22/wg21/docs/papers/2016/p0091r3.html) for functions to constructors of template classes; when you construct a class template, it is no longer necessary to specify the arguments.
* C++17 has changed the definition of qualification conversions. Previously, these were permitted between multi-level pointers and mixed pointers, such that qualifiers could often be added at levels other than the first; however, this did not similarly apply to arrays.
* Refined the [expression evaluation order](https://wg21.link/P0145R3) for major C++ operators that were previously left to compiler implementation detail, for example, member access, assignment, and array index.
* Expand the [*using* declaration](https://wg21.link/P0195R2) to support pack expansion semantics for variadic base class members, which can then be used inside the derived class.
* We are now complete with the full implementation of [Expression SFINAE](https://blogs.msdn.microsoft.com/vcblog/2016/06/07/expression-sfinae-improvements-in-vs-2015-update-3/), and made the corresponding Standard Template Library changes.
* We implemented parallel algorithms conforming to the ISO C++17 standard. See the source file located at `[VSInstallDir]\VC\Tools\MSVC\<ver>\include\yvals.h` for additional details.
* In /std:c++17 mode, the warning level of C4834 ("discarding return value of function with 'nodiscard' attribute") is increased from W3 to W1. In addition, the compiler can now deduce the type of a non-type template argument that is declared with `auto`.
* Debugging large solutions with<a id="C++P1"></a> [/Debug:fastlink](https://blogs.msdn.microsoft.com/vcblog/2016/10/05/faster-c-build-cycle-in-vs-15-with-debugfastlink/) PDBs is more robust. Changes in the PDB lead to reduced latency and a 30% reduction in heap memory consumption in the VS Debugger.
* C++ Core Check is now part of the default toolset for native code analysis. Whenever code analysis is executed over a project, a subset of rules is enabled from C++ Core Check in addition to default recommended rules.
* We added parallel compilation support for Linux projects, which may significantly improve build times. This can be enabled via **Property Pages > C/C++ > Max Number of Parallel Compilation Jobs**.
* The "Public Project Include Directories" Linux project property has been added to improve consumption of includes from project-to-project references in Linux solutions.
* We added [ClangFormat support](https://aka.ms/clangformat) for C++ developers in the IDE. Similar to EditorConfig, you can use ClangFormat to automatically style and format your code as you type, in a way that can be enforced across your development team.

### <a id="csharp"></a> C# Compiler
In addition to [bug fixes](https://github.com/dotnet/roslyn/pulls?q=is%3Apr+label%3AArea-Compilers+is%3Aclosed+milestone%3A15.7), this release brings the following C# 7.3 features:
- `System.Enum`, `System.Delegate` and [`unmanaged`](https://github.com/dotnet/csharplang/blob/master/proposals/csharp-7.3/blittable.md) constraints.
- [Ref local re-assignment](https://github.com/dotnet/csharplang/blob/master/proposals/csharp-7.3/ref-local-reassignment.md): Ref locals and ref parameters can be reassigned with the ref assignment operator (`= ref`).
- [Stackalloc initializers](https://github.com/dotnet/csharplang/blob/master/proposals/csharp-7.3/stackalloc-array-initializers.md): Stack-allocated arrays can be initialized, for example `Span<int> x = stackalloc[] { 1, 2, 3 };`.
- [Indexing movable fixed buffers](https://github.com/dotnet/csharplang/blob/master/proposals/csharp-7.3/indexing-movable-fixed-fields.md): Fixed buffers can be indexed into without first being pinned.
- [Custom `fixed` statement](https://github.com/dotnet/csharplang/blob/master/proposals/csharp-7.3/pattern-based-fixed.md): Types that implement a suitable `GetPinnableReference` can be used in a `fixed` statement.
- [Improved overload candidates](https://github.com/dotnet/csharplang/blob/master/proposals/csharp-7.3/improved-overload-candidates.md): Some overload resolution candidates can be ruled out early, thus reducing ambiguities.
- [Expression variables in initializers and queries](https://github.com/dotnet/csharplang/blob/master/proposals/csharp-7.3/expression-variables-in-initializers.md): Expression variables like `out var` and pattern variables are allowed in field initializers, constructor initializers, and LINQ queries.
-   [Tuple comparison](https://github.com/dotnet/csharplang/blob/master/proposals/csharp-7.3/tuple-equality.md): Tuples can now be compared with `==` and `!=`.
-   [Attributes on backing fields](https://github.com/dotnet/csharplang/blob/master/proposals/csharp-7.3/auto-prop-field-attrs.md): Allows `[field: …]` attributes on an auto-implemented property to target its backing field.

### <a id="Python"></a> Python
 - You can run MyPy on a project by right-clicking on the project and selecting **Python > MyPy**. MyPy will check your code against type hints, and any type errors detected will be shown in the error list.
 - You can create and use Conda environments as well as manage packages for your Conda environments using pip or Conda. 
 - Anaconda version 5.1.0 is now available from the Visual Studio Installer and is installed by default when the Data Science workload is selected.
 - We added an opt-in to the ptvsd 4.0 version of the Python debugger based on the popular open source [pydevd debugger](https://pypi.python.org/pypi/pydevd/). The opt-in offers faster debugging performance for applicationscan and can be enabled by checking **Use experimental debugger** from **Tools > Options > Python > Experimental**. 
 - Check out the [Python in Visual Studio 15.7 blog post](https://aka.ms/Jpr4b7) for more on using the debugger, Conda, MyPy, and type hints.

### <a id="xamarin"></a> Visual Studio Tools for Xamarin
This release includes [Xamarin.Android 8.3](https://developer.xamarin.com/releases/android/xamarin.android_8/xamarin.android_8.3/) and [Xamarin.iOS 11.10](https://developer.xamarin.com/releases/ios/xamarin.ios_11/xamarin.ios_11.10/).

#### <a id="android-auto-sdk"></a>Automatic Android SDK Management
When a Xamarin.Android project is loaded, Visual Studio can determine if the Android API level used by the project is missing from your machine and automatically install it for you in the background. To enable this feature, go to **Tools > Options > Xamarin > Android Settings > Auto Install Android SDKs**.

#### <a id="xamarin-intellisense"></a> Improved XAML IntelliSense
Xamarin.Forms developers using Visual Studio 2017 version 15.7 will notice a vastly improved IntelliSense experience _(Figure 5)_. The Xamarin.Forms XAML editing experience is now powered by the same IntelliSense engine that powers WPF and UWP. This brings many enhancements to developers, including improved matching, light bulb suggestions, code navigation, linting, resource completion, and markup extension completion.
<figure><center><img src="media/xamarin-forms-intellisense.gif" alt="Xamarin.Forms XAML editing experience"><figcaption><em>(Figure 5) Xamarin.Forms XAML editing experience</em></figcaption></center></figure>

#### <a id="xaml"></a>Tooling Enhancements for Conditional XAML
The XAML editor provides IntelliSense for authoring [conditional XAML](https://docs.microsoft.com/en-us/windows/uwp/debug-test-perf/conditional-xaml). When using a type that is not present in the target min version of your app, the XAML editor now not only warns, but also, provides several options to fix it. 

#### <a id="xamarin-provisioning"></a> Automatic iOS Provisioning
We made iOS device provisioning for development easier _(Figure 6)_. In Visual Studio 2017 version 15.7, there's a streamlined experience to request a development certificate, generate a signing key, add a device in the Developer Center, and create a provisioning profile, all with a single button click. All the heavy lifting of provisioning an iOS device is handled for you in less than 30 seconds.

<figure><center><img src="media/iOS-Provisioning.gif" alt="iOS & Android Project Templates"><figcaption><em>(Figure 6) Provisioning iOS apps got easier with our automatic iOS provisioning feature.</em></figcaption></center></figure>

#### <a id="xamarin-sdkmanagement"></a> Android SDK Management
Figuring out what Android SDKs to install for mobile development can be time consuming. Visual Studio 2017 version 15.7 adds a new Android SDK manager that takes the guesswork out of managing Android SDK installations. After opening a project for which you don’t have SDKs installed to build it, a notice will appear to help you download the required SDKs. After clicking **Download & Instal** and accepting the relevant license agreement, the correct SDKs will automatically be installed in the background for you.

#### <a id="xamarin-templates"></a> New iOS & Android Project Templates
Whether you’re a new or seasoned Xamarin developer, project templates are an important part of the app building journey. They should be easy to find and set you up for success from the start _(Figure 7)_. In this release, we completely [rebuilt our iOS and Android native project templates](https://blog.xamarin.com/new-xamarin-android-ios-templates/) for better discoverability and support for modern navigation patterns like flyout or bottom tabs.
<figure><center><img src="media/xamarin_android-nav-drawer.gif" alt="iOS & Android Project Templates"><figcaption><em>(Figure 7) Easy to find and set your iOS & Android Project Templates</em></figcaption></center></figure>

#### <a name="improvements-to-installation"></a>Improvements to Installation
The Visual Studio Installer ships with an updated Android SDK configuration, including Android API 27 and Android SDK Tools 26. This includes support for [quick boot](https://blog.xamarin.com/android-emulator-quick-boot/), which enables your Android emulator to boot in less than five seconds.

Additionally, we include the [Android Device Manager](https://docs.microsoft.com/en-us/xamarin/android/get-started/installation/android-emulator/xamarin-device-manager?tabs=vswin) as part of the Mobile development with .NET workload to easily create, edit, and delete emulators.

#### <a id="dotnet_productivity"></a> .NET Productivity Improvements
- Use *Quick Actions and Refactorings* (**Ctrl+.**) to:
    - Convert `for`-to-`foreach`, and vice versa.
  - Make private fields `readonly`.
- Go To Definition (**F12**) is now supported for LINQ query clauses and deconstructions.
<a id="dotnet_tooling"></a>
* Use **Ctrl+.** to toggle between `var` and the explicit type, regardless of your code style preferences.
* Quick Info shows captures on lambdas and local functions, so you can see what variables are in scope.
* *Change Signature* refactoring (**Ctrl+.** on signature) works on local functions.
* You can edit .NET Core project files in-place, so opening containing folder, restoring tabs, and other Editor features are fully supported. IDE changes, such as adding a linked file, will be merged with unsaved changes in the editor.

### <a id="test"></a>Testing
* Live Unit Testing works with embedded pdbs and pdbs specifying /deterministic.
* We added Live Unit Testing support for projects that use reference assemblies.
* The Test Explorer<a id="TestExplorer"></a> has more responsive icons during test runs. When a test run is in progress, a progress ring appears next to tests that are currently executing, and a clock icon appears for tests that are pending execution.

### <a id="webtools"></a>Web Tools
* The ASP.NET Web Application project templates have been refreshed to newer versions of the dependent packages.
* You can<a id="ASP.NET"></a> publish your non-containerized applications to Azure App Service on Linux.
* Link to open your Azure App Service in Cloud Explorer from the Publish Summary page.
* You have support for publishing .NET Core framework dependent and self-contained applications.
* Publish support for F# applications to App Service and folder.
*   We added support for hosing ASP.NET Core applications directly in the IIS Express process.
*   You can create a storage account and provide a connection string name to be stored in App Service settings when publishing to a new Azure App Service.
* We improved Kestrel HTTPs support during debugging. 
* ASP.NET Core applications support multiple semi-colon separated values in the "App URL" field under project properties. When multiple URLs are present in this field, the first one is used to launch the browser.
* New scaffolder called "Identity" is available via the command line (GUI support coming soon), which adds identity management UI to your ASP.NET Core 2.1 applications.
<a id="KeyVault"></a>
* ASP.NET and ASP.NET Core projects can create and associate Azure Key Vaults with their web applications within the IDE by configuring the "Key Vault" Connected Service.
* When an ASP.NET or ASP.NET Core application depends on Azure Key Vault, an error appears in the error list if the app is unable to access that Key Vault at runtime from the developer’s machine given the account selected under **Tools > Options > Azure Service Authentication**. This shortens the time to discover and correct the permission or account issue and avoid an application failure at runtime.
* When your web app consumes a KeyVault to which your selected ASAL user account has no access, a warning will now appear in the Error List.

### <a id="BuildTools"></a>Visual Studio 2017 Build Tools 
#### <a name="support-for-azure-uwp-and-other-workloads"></a>Support for Azure, UWP, and Other Workloads
Visual Studio 2017 Build Tools support command-line builds for most Visual Studio projects. Supported projects include: ASP.NET, Azure, C++ desktop, ClickOnce, containers, .NET Core, .NET Desktop, Node.js, Office and SharePoint, Python, TypeScript, Unit Tests, UWP, WCF, and Xamarin. We expect to add support for SQL in a future release. Visual Studio Build Tools now also support [installing into a container](https://docs.microsoft.com/visualstudio/install/build-tools-container). You can download Visual Studio Build Tools from [Visual Studio Downloads](https://www.visualstudio.com/downloads/#build-tools-for-visual-studio-2017).
A list of workload and component IDs with which you can tailor your container image can be found in the [Visual Studio Build Tools 2017 component directory](https://docs.microsoft.com/visualstudio/install/workload-component-id-vs-build-tools).

> [!NOTE]
> Build Tools requires a license to Visual Studio 2017.

#### <a id="BuildToolsUWP"></a> UWP Support in Visual Studio 2017 Build Tools
Visual Studio Build Tools allow you to create build servers without installing all of Visual Studio. In response to customer requests, we enhanced Visual Studio Build Tools to support additional project types. These project types include UWP tools, bringing the supported project list ASP.NET, Azure, C++ desktop, ClickOnce, containers, .NET Core, .NET Desktop, Node.js, Office and SharePoint, Python, TypeScript, Unit Tests, UWP, WCF, and Xamarin. We expect to add support for SQL in a future release.

### <a id="WinTools"></a> Tools for Universal Windows Platform Developers
* Visual State Management and Animation tooling is available in Blend with the latest updates to the XAML Designer. All UWP developers have access to these tools. In addition, XAML Edit & Continue supports editing Visual States and Animations.
* [Windows Machine Learning automatic code generation](https://docs.microsoft.com/en-us/windows/uwp/machine-learning/overview#automatic-interface-code-generation) support allows WinML wrapper classes to be generated by adding your ONNX model files as an existing item in the project.
* The Windows 10 April 2018 Update SDK (Build 17134) is the default SDK for the Universal Windows Platform development workload in Visual Studio.
* You can create [related sets](https://docs.microsoft.com/windows/uwp/packaging/optional-packages) with code execution in optional packages using C# and the new Optional Code Package project template.
* With the new 'Package Layout' item template, you can easily construct [flat package bundles](https://docs.microsoft.com/windows/uwp/packaging/flat-bundles). 

#### <a id="appinstaller"></a>AppInstaller Support in APPX Packages
The Universal Windows Platform allows distributing applications without the Microsoft Store by using a mechanism called “sideloading”. This release allows you to generate the appinstaller file to get automatic updates from your APPX based deployments. Learn more about the [underlying technology](https://docs.microsoft.com/en-us/windows/uwp/packaging/appinstaller-root).

### <a id="nugetpreview3"></a> NuGet 
* This release provides out of the box support for [migrating existing projects based on `packages.config` to `PackageReference`](https://aka.ms/nuget-migrator-docs).

* We added support for<a id="NuGet"></a> NuGet package signatures. Installing or restoring [signed packages](https://aka.ms/nuget-signatures) validates the digital signature before extracting the packages content. If the signature validation fails (for example, the content has been tampered with, invalid certificate, etc.) the operation will be blocked with a build error that is shown in the Error List.

### <a id="TypeScript-JavaScript"></a>TypeScript and JavaScript
TypeScript 2.8 RC is now included in Visual Studio 2017 version 15.7.  
This release brings the following improvements:
* **Support for `jsconfig.json`**, a file that can help control your editor options much like `tsconfig.json`.
* An option to reduce resource usage by **turning off type-checking for unopened files**.
  * This is the *only report diagnostics for files opened in the editor* option under **Tools > Options > TextEditor > JavaScript/TypeScript > Project**.
* **New editing features** for both TypeScript and JavaScript users:
  * Applying all quick fixes within a file.
  * Organize imports.
  * Completions for `this.` in classes and braces in JSX.
* **TypeScript 2.8** features:
  * Conditional types (`A extends B ? C : D`).
  * New `lib.d.ts` conditional type helpers such as `NonNullable`, `ReturnType`, `Extract`, and `Exclude`.
  * Granular control on modifiers in mapped types.
  * Control on JSX factories within files using the new `// @jsx` pragma.

You can find more information on TypeScript 2.8 in the [TypeScript 2.8 RC blog](https://blogs.msdn.microsoft.com/typescript/2018/03/15/announcing-typescript-2-8-rc/).  
* **TypeScript 2.7** features:
  * Strict property initialization.
  * Numeric separators.
  * Smarter type guards.
  
You can find more information on TypeScript 2.7 in the [TypeScript 2.7 blog](https://blogs.msdn.microsoft.com/typescript/2018/01/31/announcing-typescript-2-7/).

We also fixed some of the top issues raised by customers, including premature triggering of snippets, uncancellable refactorings, hard-to-disable formatting, and incorrect TypeScript version selection. 

> [!NOTE]
> These improvements are powered by TypeScript 2.8. For the best experience, update your existing projects to the latest TypeScript version.

###  <a id="Edge"></a> JavaScript debugging with Microsoft Edge
Visual Studio ASP.NET and .NET core developers on Windows Insider builds, can set breakpoints and debug their JavaScript files using a Microsoft Edge browser. Visual Studio will use the new [Edge DevTools Protocol](https://docs.microsoft.com/en-us/microsoft-edge/devtools-protocol/0.1/) developed by the Microsoft Edge team when targeting Microsoft Edge browser. Developers can debug and fix JavaScript issues from within Visual Studio in both Microsoft Edge and Google Chrome browsers. We are glad to enable this often-requested feature from our customers. We would love to hear your feedback on the feature to help us improve and build a better Visual Studio.

### <a id="debug"></a> Debugging and Diagnostics
This release adds VSTS and GitHub authentication support for Source Link. <a id="debug2"></a>Authentication will be added to Source Link requests automatically if it is available through the IDE. If the user is not already authenticated, the sign in UI will be shown to enable authentication.

IntelliTrace’s [step-back debugging feature](https://docs.microsoft.com/en-us/visualstudio/debugger/how-to-use-intellitrace-step-back) is supported for debugging .NET Core projects. 
  * To enable the feature, go to<a id="debug3"></a> **Tools > Options > IntelliTrace settings**, and select the **IntelliTrace events and snapshots** option. 
* IntelliTrace's [step-back debugging feature](https://docs.microsoft.com/en-us/visualstudio/debugger/how-to-use-intellitrace-step-back) supports taking snapshots on exceptions. To enable the feature, go to **Tools > Options > IntelliTrace settings**, and select the option **IntelliTrace events and snapshots** _(Figure 8)_.

<figure><center><img src="media/snapshotOnException.PNG" alt="Snapshot on exception"><figcaption><em>(Figure 8) Snapshot on exception</em></figcaption></center></figure>

### <a name="launch-and-attach-script-debugger-to-microsoft-edge-for-aspnet-projects"></a>Launch and Attach Script Debugger to Microsoft Edge for ASP.NET Projects
  You can debug both JavaScript and TypeScript directly in Visual Studio when using Google Chrome as your browser of choice. All you need to do is select Chrome as your browser in Visual Studio and hit F5 to debug.
See the [Client-side debugging of ASP.NET projects in Google Chrome](https://blogs.msdn.microsoft.com/webdev/2016/11/21/client-side-debugging-of-asp-net-projects-in-google-chrome/) for additional information.

### <a id="te"></a>Team Explorer
In **Git Settings**, **Global Settings** in Team Explorer, there is an option to choose between OpenSSL and Secure Channel. OpenSSL is the default.

### <a id="SFTools"></a> Service Fabric Tooling for the 6.2 Service Fabric release
The Service Fabric Tools for the <a href="https://blogs.msdn.microsoft.com/azureservicefabric/2018/04/19/service-fabric-6-2-release/" target="blank">Service Fabric 6.2 release</a> provide compatibility support for the 6.2 runtime and 3.1 SDK. Along with several bug fixes, a new feature enables adding container support to existing ASP.NET or Console projects.  Both .NET Framework and .NET Core 2.0 projects are supported through a new "Add Orchestration Support" context menu and dialog.  Once these projects have added Service Fabric orchestration support, they can be deployed remotely and debugged on the local Service Fabric cluster.   

### <a id="EFTools"></a> Entity Framework Tools Improvements
* Support for the [Entity Framework 6.2 Runtime](https://blogs.msdn.microsoft.com/dotnet/2017/10/26/entity-framework-6-2-runtime-released/): Creating an EF model in a project that does not reference EF will now install the [EF 6.2 NuGet package](https://www.nuget.org/packages/EntityFramework/6.2.0) by default.
* Various accessibility improvements in the EF Designer and Wizard.
* [Significantly faster reverse engineering using recent versions of SQL Server](https://github.com/aspnet/EntityFramework6/issues/4).
* [Support for updating models from SQL Server databases with more than 300 tables](https://github.com/aspnet/EntityFramework6/issues/185).
* [Support for reverse engineering UNION views on Oracle databases](https://github.com/aspnet/EntityFramework6/issues/243).

### <a id="fsharp"></a> F\# and F\# Tools Improvements

We made many improvements to F# and its tools. Performance and cleaning up existing experiences with .NET SDK-style projects has been the focus for this release. As always, we also received significant contributions from the wonderful F# community.

#### <a name="f-compiler-and-core-library-improvements"></a>F\# Compiler and Core Library Improvements

* Enabled generating F# AssemblyInfo from properties with the F# compiler in the .NET SDK.
* `--debug:full` is supported for the F# .NET Core compiler on Windows.
* `MakeTuple` is supported for struct tuples.
* An [unnecessary warning](https://github.com/Microsoft/visualfsharp/issues/4386) when using an extension method for a tuple is now resolved.
* `MailboxProcessor.PostAndAsyncReply` properly handles cancellation when a parent process is cancelled.
* Equality for `float32` types is now correct when `NonStructuralComparison` is used.
* Warnings are now forwarded when searching for method overloads, by [Matthias Dittrich](https://github.com/matthid).
* An [improvement to a warning when pattern matching on an enum](https://github.com/fsharp/fslang-suggestions/issues/652) to emit an example of an unmatched enum, by [John Wostenberg](https://github.com/jwosty).

#### <a name="f-tooling-improvements"></a>F\# Tooling Improvements

* Significant reductions in memory usage in the F# Compiler Service, by [Avi Avni](https://github.com/aviavni) and Microsoft.
* Significant performance improvements for the Unused Open Analyzer when it is turned on.
* Improved responsiveness when F# analyzers and code fixes are turned on, such that error diagnostics are always prioritized above the rest.
* We added ASP.NET Core templates for F#.
* The initial ordering for pasted files in folders for .NET SDK projects is now correctly at the top of the scope the file was pasted into.
* F# scripts without a project file correctly sends code to F# Interactive when **Alt+Enter** is pressed.
* The debugger view for F# lists has been extended from 50 items to 5000 items.
* Classic F# projects (.NET Framework only) also perform design-time builds, which reduces solution load time.
* The Structured Guidelines and Outlining views can now be toggled, under **Settings > Text Editor > F# > Advanced**.
* Assembly level attributes are now returned by the F# Compiler Service.
* We added `Entity.DeclaringEntity` to the F# Compiler Service.
* Optimization is available via the F# Compiler Service API, by [Steffen Forkmann](https://github.com/forki) and [ncave](https://github.com/ncave).
* `GetDeclarationLocation` no longer requires a file to provide results on otherwise correct data, by [amieres](https://github.com/amieres).
* `IsNameGenerated` is now available in the F# Symbols API, by [Eugene Auduchinok](https://github.com/auduchinok).

#### <a name="f-infrastructure-improvements"></a>F\# Infrastructure Improvements

* `autoconf` is no longer required in our Mono build.
* All Visual Studio integration projects now use the .NET SDK.
* The commit hash for a build of the tools is available in **Help > About Microsoft Visual Studio**.

To see the full commit log of what went into this release, check out [our release tag for 15.7](https://github.com/Microsoft/visualfsharp/releases/tag/Visual-Studio-2017-Version-15.7).

<hr style="border:1px solid Silver">

## <a id = "knownissues"></a> **Known Issues**

See all existing known issues and available workarounds in Visual Studio 2017 version 15.7.

<a href="https://developercommunity.visualstudio.com/topics/Known+Issue+in%3A+Visual+Studio+2017+Version+15.7.html" target="blank"> <img src="media/Known_Issues_button2.svg" alt="Visual Studio 2017 Known Issues"></a>

<hr style="border:1px solid Silver">

## <img src="media/News_icon.svg" alt="Release Notes Icon"> <a id="15.7.1"></a>Visual Studio 2017 version 15.7.1 <img src="media/New_button_bg2.svg" alt="New Release icon">
_released on May 08, 2018_

## <a name="top-issues-fixed-in-1571"></a>**Top Issues Fixed in 15.7.1**
These are the customer-reported issues addressed in 15.7.1: 
* This release includes a fix that reduces memory usage and GC pressure during solution load.

<hr style="border:1px solid Silver">

## <img src="media/News_icon.svg" alt="Release Notes Icon"> </a> Visual Studio 2017 version 15.7 Security Advisory Notice <a id="15.7.S"></a> <img src="media/New_button_bg2.svg">
_updated on May 08, 2018_

### <a name="microsoft-security-advisory-for-net-core-denial-of-service-vulnerability"></a>Microsoft Security Advisory for .NET Core Denial Of Service Vulnerability
**CVE-2018-0765**

Microsoft is releasing this security advisory to provide information about a vulnerability in .NET Core and .NET native version 2.0. This advisory also provides guidance on what developers can do to update their applications to remove this vulnerability.

Microsoft is aware of a denial of service vulnerability that exists when .NET Framework and .NET Core improperly process XML documents. An attacker who successfully exploited this vulnerability could cause a denial of service against a .NET Framework, .NET Core, or .NET native application.

The update addresses the vulnerability by correcting how .NET Framework, .NET Core, and .NET native applications handle XML document processing.

If your application is an ASP.NET Core application, developers are also advised to update to ASP.NET Core 2.0.8.

<hr style="border:1px solid Silver">

## <a name="feedback"></a>**Feedback**
We’d love to hear from you! For issues, let us know via the <a href="https://docs.microsoft.com/visualstudio/ide/how-to-report-a-problem-with-visual-studio-2017" target="blank">Report a Problem</a> option in the upper right-hand corner of either the installer or the Visual Studio IDE itself. The <img src="media/Feedback_icon-2.png" alt="Feedback Icon"> icon is located in the upper right-hand corner. You can track your issues in the <a href="https://developercommunity.visualstudio.com" target="blank">Visual Studio Developer Community</a>, where you can ask questions and find answers. You can also make a product suggestion through <a href="https://visualstudio.uservoice.com/forums/121579-visual-studio-ide" target="blank">UserVoice</a> or get free installation help through our <a href="https://www.visualstudio.com/vs/support/#talktous" target="blank">Live Chat support</a>. 

<hr style="border:1px solid Silver">

## <a name="blogs"></a>**Blogs**

Take advantage of the insights and recommendations available in the Developer Tools Blogs site to keep you up-to-date on all new releases and include deep dive posts on a broad range of features. 

<a href="https://blogs.msdn.microsoft.com/developer-tools/" target="blank"><img src="media/Blogs_button3.svg" alt="Developer Tools Blogs"></a>

<hr style="border:1px solid Silver">

## <a name="visual-studio-2017-release-notes-history"></a>**Visual Studio 2017 Release Notes History**
You can view prior versions of Visual Studio 2017 release notes:

* <a href="https://docs.microsoft.com/visualstudio/releasenotes/vs2017-relnotes-v15.6" target="blank">Visual Studio 2017 version 15.6</a>
* <a href="https://docs.microsoft.com/visualstudio/releasenotes/vs2017-relnotes-v15.5" target="blank">Visual Studio 2017 version 15.5</a>
* <a href="https://docs.microsoft.com/visualstudio/releasenotes/vs2017-relnotes-v15.4" target="blank">Visual Studio 2017 version 15.4</a>
* <a href="https://docs.microsoft.com/visualstudio/releasenotes/vs2017-relnotes-v15.3" target="blank">Visual Studio 2017 version 15.3</a>
* <a href="https://docs.microsoft.com/visualstudio/releasenotes/vs2017-relnotes-v15.2" target="blank">Visual Studio 2017 version 15.2</a>
* <a href="https://docs.microsoft.com/visualstudio/releasenotes/vs2017-relnotes-v15.1" target="blank">Visual Studio 2017 version 15.1</a>
* <a href="https://docs.microsoft.com/visualstudio/releasenotes/vs2017-relnotes-v15.0" target="blank">Visual Studio 2017 version 15.0</a>

<hr style="border:1px solid Silver">

<center><a href="#top" data-raw-source="[Top of Page](#top)">Top of Page</a></center>

<a id="bottom"></a>
