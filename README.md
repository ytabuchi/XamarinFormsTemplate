# XamarinFormsTemplate

This is source code of newest Xamarin.Forms Template made by Japan Xamarin User Group.

# How to get

### Option 1: Clone the Repository (Recommended)

Clone the project on the following location directly:

```%USERPROFILE%\Documents\Visual Studio 2015\Templates\ProjectTemplates\Visual C#```

That is, on a command prompt, you can install the template by the following commands:

```
cd "%USERPROFILE%\Documents\Visual Studio 2015\Templates\ProjectTemplates\Visual C#"
git clone https://github.com/ytabuchi/XamarinFormsTemplate.git
```

After the first installation, you can of course update your copy by ```git pull``` and you feel it's easier to update the templates than the other option.

### Option 2: Download the ZIP

- Download XamarinFormsTemplate-master.zip file from [GitHub](https://github.com/ytabuchi/XamarinFormsTemplate/archive/master.zip)
- Extract the zip file
- Move the extracted ```XamarinFormsTemplate-master``` folder to the following location:
```%USERPROFILE%\Documents\Visual Studio 2015\Templates\ProjectTemplates\Visual C#```


<img src="https://github.com/ytabuchi/XamarinFormsTemplate/blob/master/NewProject.png" alt="New project dialog" width="450" />

Please see [blog page (in Japanese)](http://ytabuchi.hatenablog.com/entry/vs-xf-template) for how to use.

# Notices when using

- When generating a project, you will see the following dialog message. Please select "Reload all".

<img src="https://github.com/ytabuchi/XamarinFormsTemplate/blob/master/01-Android_warning.png" alt="Android Warning" width="300" />

- After project is generated, you have to "Restore NuGet packages".

<img src="https://github.com/ytabuchi/XamarinFormsTemplate/blob/master/02-RestoreNuGet.png" alt="Android Warning" width="300" />

- Then restart Visual Studio. Some warning might be remained, but no error will be remained.


# How to maintenance

`MyTemplate.vstemplate` located in Root folder is a Master file that is specify each child projects.
In each projects folder, there are `MyTemplate.vstemplate` files. They are the template setting files for each projects.

If Xamarin.Forms will be updated, you can just change the version numbers of each `MyTemplate.vstemplate` files

There are some macros in the template files. Please see [MSDN document](https://msdn.microsoft.com/ja-jp/library/eehb4faa.aspx) for each meaning.
