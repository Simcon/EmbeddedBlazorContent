# EmbeddedBlazorContent

This library helps you in server Blazor mode to enable content files from BlazorLib projects.
In my opinion at this moment it is the perfomance and convenient way use embedded content files from Blazor Libraries.

## Usage

- Install latest version from nuget

- Enable Host return static content from embedded resources.
```
# Startup.cs
app.UseEmbeddedBlazorContent(assembly);

// or with custom requestPath

app.UseEmbeddedBlazorContent(assembly, "/staticContent");
```

- Include links to static content in page
```html
# _Host.cshtml
@Html.EmbeddedBlazorContent(assembly)

// or with custom requestPath

@Html.EmbeddedBlazorContent(assembly, "/staticContent")

// or all embedded content from all hosted asemblies

@Html.EmbeddedBlazorContent()
```

## Examples
- EmbeddedBlazorContent.ExampleApp
- EmbeddedBlazorContent.ExampleLib

## License
[MIT](LICENSE)
