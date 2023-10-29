> 1 / 1
>
> mkdocs material costume css

1 / 1

If you want to customize the appearance of your MkDocs Material theme documentation site by applying custom CSS, you can follow these steps:

1. **Create a `custom.css` File:**

    First, create a custom CSS file (e.g., `custom.css`) where you will define your custom styles. You can create this file in your project's root directory or in a specific folder, depending on your preference.

2. **Edit Your `mkdocs.yml` Configuration:**

    Open your `mkdocs.yml` configuration file, and add or modify the following lines:

yaml

```yaml
theme:
  name: "material"
  custom_dir: "path_to_custom_css_folder" # Optional
```

    Replace `'path_to_custom_css_folder'` with the relative path to the folder where your `custom.css` file is located. If you placed the `custom.css` file in your project's root directory, you can omit the `custom_dir` setting.

3. **Reference the Custom CSS in Your HTML Template:**

    To include your custom CSS file in the generated documentation, you need to modify the HTML template. You can either create a custom template or directly modify the existing template used by the Material theme.

    To create a custom template, you can use the `md_template_dir` option in your `mkdocs.yml`:

    yaml

    ```yaml
    markdown_extensions:
      - markdown_include.include
    md_template_dir: "path_to_custom_template_folder"
    ```

    Then, in your custom template folder, create an `extra_head.html` file, which will be included in the `<head>` section of each page. Inside this file, link to your custom CSS file:

    html

    ```html
    <link rel="stylesheet" href="{{ config.theme.custom_dir }}/custom.css" />
    ```

4. **Apply Custom Styles:**

In your `custom.css` file, you can add custom CSS styles to modify the appearance of your documentation. You can use CSS rules to target specific elements or classes and define your desired styles.

For example, to change the background color of code blocks, you can use CSS like this:

css

```css
pre {
  background-color: #f2f2f2;
}
```

5. **Build Your Documentation:**

    After making these changes, rebuild your documentation site by running the `mkdocs build` command.

6. **View Your Customized Documentation:**

    Once the build process is complete, you can view your documentation with the custom CSS styles applied.

Keep in mind that customizing the appearance of your MkDocs Material theme documentation site using CSS allows you to tailor the design to your specific needs. You can modify fonts, colors, layout, and more to match your branding or improve the user experience.
