# C# Project Templates

These templates are designed to help you get started with new projects quickly and efficiently.

## Installation

To install a template globally on your machine:

1. Open your terminal and navigate to the root directory of the template you want to install.
2. Run the following command:

    ```bash
    dotnet new -i .
    ```

This will install the template, making it available for use in any directory on your machine.
To see all the available templates, run: ```dotnet new --list```

## Usage

Once a template is installed, you can create a new project based on the template by running:

```bash
dotnet new <shortName> -n <DesiredProjectName>
```

- Replace `<shortName>` with the template's short name (found in the `template.json` file).
- Replace `<DesiredProjectName>` with the name of your new project.

This command will generate a new project directory with the specified name, using the installed template's structure and configuration.

## Contributing

Help improve these templates or add new ones! Here’s how you can contribute:

1. **Create a New Template**:
    - Navigate to the root directory of the repository.
    - Create a new directory for your template:

        ```bash
        mkdir <NewTemplateName>
        cd <NewTemplateName>
        ```

    - Inside this new directory, set up your project as you normally would, including any files, folders, or configurations that should be part of the template.

2. **Configure the Template**:
    - Create a `.template.config` directory inside the root of your new template:

        ```bash
        mkdir .template.config
        ```

    - Inside the `.template.config` directory, create a `template.json` file:

        ```bash
        touch .template.config/template.json
        ```

    - Populate the `template.json` file with metadata that defines your template. Refer to existing templates for examples of what to include.

3. **Test Your Template**:
    - Navigate to the root directory of your new template.
    - Install it locally using `dotnet new -i .` and test its functionality by creating a new project using the installed template.