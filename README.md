# XamarinFormsTemplate

This is source code of newest Xamarin.Forms Template made by Japan Xamarin User Group.

# How to use

1. Download or fork this repository.
2. Extract downloaded .zip file.
3. In extracted folder that is named `XamarinFormsTemplate-master`, zip all files and folders to your preferred name.
4. Locate the .zip file to `Visual Studio project folder\Templates\ProjectTemplates\Visual C#`.
5. Try create a new project. you can see the below.



Please see [blog page (in Japanese)](http://ytabuchi.hatenablog.com/entry/vs-xf-template) for how to use.


# How to maintenance

`MyTemplate.vstemplate` located in Root folder is a Master file that is specify each child projects.
In each projects folder, there are `MyTemplate.vstemplate` files. They are the template setting files for each projects.

If Xamarin.Forms will be updated, you can just change the version numbers of each `MyTemplate.vstemplate` files

There are some macros in the template files. Please see [MSDN document](https://msdn.microsoft.com/ja-jp/library/eehb4faa.aspx) for each meaning.
