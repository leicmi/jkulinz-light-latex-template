# ![LightLogo](./images/header_logo.svg)

A minimal repository containing the JKU Linz Light report template which can be
integrated into other repositories as a submodule. The benefit of using this
submodule is the ability to receive updates directly. For a full list of
features, changelog, as well as examples of this LaTeX template please visit
the main [`jkulinz-light-latex-template](https://github.com/leicmi/jkulinz-light-latex-template)
repository.

## Installation

To use this repository as a submodule a `.gitmodules` file must be defined in
the parent repository with the following contents:

```gitconfig
[submodule "jkulinz-light"]
    path = jkulinz-light
    url = https://github.com/leicmi/jkulinz-light-latex-template.git
    branch = main-template
```

The easiest way to generate this file as well as clone the template is to run
the following command:

```bash
git submodule add -b main-template https://github.com/leicmi/jkulinz-light-latex-template.git jkulinz-light
```

If desired, the template can be added into a subdirectory, i.e a `docs/` folder
as follows:

```bash
git submodule add -b main-template https://github.com/leicmi/jkulinz-light-latex-template.git docs/jkulinz-light
```

## Updating

Once the submodule is installed, the following command will fetch the
newest version of the template:

```bash
git submodule update --recursive --remote
```

If you have other submodules in the parent repository and only want to update
the template, then use the following command:

```bash
git submodule update --remote tulinz-light
```

**Note:** If the `docs/` subdirectoy method was used when installing the
template, the above command will become:

```bash
git submodule update --remote docs/tulinz-light
```
