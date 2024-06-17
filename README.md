## Blazorise.Modal Issue Demonstration (v1.5.3)
This repository is created to demonstrate an issue encountered when opening the Blazorise.Modal component in version 1.5.3. It includes a minimal example to reproduce the error for debugging and reporting purposes.

### Steps to Set Up the Project
1. Create a Blazor Server App: Start by creating a new Blazor Server application.

2. Add NuGet Package References: Add the following package references to your project file:

```xml
<PackageReference Include="Blazorise" Version="1.5.3" />
<PackageReference Include="Blazorise.Bootstrap5" Version="1.5.3" />
<PackageReference Include="Blazorise.Components" Version="1.5.3" />
<PackageReference Include="Blazorise.DataGrid" Version="1.5.3" />
<PackageReference Include="Blazorise.Icons.FontAwesome" Version="1.5.3" />
<PackageReference Include="Blazorise.Snackbar" Version="1.5.3" />
<PackageReference Include="Blazorise.FluentValidation" Version="1.5.3" />
```

3. Configure Services: In your Program.cs or Startup.cs, configure the Blazorise services:

```c#
builder.Services.AddBlazorise();
builder.Services.AddBootstrap5Providers();
builder.Services.AddFontAwesomeIcons();
builder.Services.AddBlazoriseFluentValidation();
```

4. Add css reference
```html
<link href="_content/Blazorise/blazorise.css" rel="stylesheet" />
```

5. Create a Basic Modal Component: Create a new component named SampleModal.razor with a basic modal implementation.

6. Modify Index.razor: Update the Index.razor file to call and display the modal component.

By following these steps, you will have a minimal project setup to reproduce the issue with the Blazorise.Modal component in version 1.5.3.