# XamarinFormsTemplate

This is source code of newest Xamarin.Forms with .NET Standard Xamarin.Forms core project Template by Japan Xamarin User Group.

## Specification

- Xamarin.Forms 3.5.0.129452
- PackageReference (can use only Visual Studio 2017)
- .NET Standard 2.0 core project

## Note

- This template use Xamarin.Android.Support Library v27.0.2.1, so that you need Android SDK Platform v27 or higher to build.

# How to get

### Option 1: Clone the Repository (Recommended)

Clone the project on the following location directly:

`%USERPROFILE%\Documents\Visual Studio 2017\Templates\ProjectTemplates\Visual C#`

or make `Cross-Platform` directory in the above directory, then clone this repogitory.

From command prompt, you can install the template by the following commands:

```
cd "%USERPROFILE%\Documents\Visual Studio 2017\Templates\ProjectTemplates\Visual C#"
git clone https://github.com/ytabuchi/XamarinFormsTemplate.git
```

After the first installation, you can update your copy by `git pull` in `XamarinFormsTemplate` directory, and you feel it's easier to update the templates than the other option.

### Option 2: Download the ZIP

- Download XamarinFormsTemplate-master.zip file from [GitHub](https://github.com/ytabuchi/XamarinFormsTemplate/archive/master.zip)
- Extract the zip file
- Move the extracted `XamarinFormsTemplate-master` folder to the following location:
`%USERPROFILE%\Documents\Visual Studio 2017\Templates\ProjectTemplates\Visual C#`

Please see [blog page (in Japanese)](http://ytabuchi.hatenablog.com/entry/vs-xf-template) for how to use.

# How to use

In this template, the Bundle ID base name is set `org.jxug.PROJECTNAME`.If you want to use your own Bundle ID base name such as `com.yourcompany.PROJECTNAME`, please follow the instructions below:

- Android
    - Oepn `Properties\AndroidManifest.xml`, then change `package="org.jxug.$ext_safeprojectname$"`.
    - `$ext_safeprojectname$` will be replaced with a new project name that you input in "New project" window.
- iOS
    - Open `Info.plist`, then change `<string>org.jxug.$ext_safeprojectname$</string>`.
    - `$ext_safeprojectname$` will be replaced with a new project name that you input in "New project" window.
- UWP
    - UWP package name will be set from UUID, so that you need nothing to do.

# How to maintenance

`MyTemplate.vstemplate` located in Root folder is a Master file that is specify each child projects.
In each projects folder, there are `MyTemplate.vstemplate` files. They are the template setting files for each projects.

If Xamarin.Forms will be updated, you can just change the version numbers of each `MyTemplate.vstemplate` files

There are some macros such as `WizardExtension` in the template files. Please see [MSDN document](https://docs.microsoft.com/en-us/visualstudio/extensibility/visual-studio-template-schema-reference) for each meaning.
