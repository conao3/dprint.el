# dprint.el

Emacs integration for [dprint](https://dprint.dev/), a fast and pluggable code formatter.

## Overview

dprint.el provides seamless code formatting in Emacs using the dprint formatter. dprint is known for its speed and extensive plugin ecosystem, supporting TypeScript, JavaScript, JSON, Markdown, TOML, and many other formats.

## Requirements

- Emacs 25.1 or later
- [dprint](https://dprint.dev/install/) installed and available in your PATH

## Installation

### Using package.el

```elisp
(package-install 'dprint)
```

### Using use-package

```elisp
(use-package dprint
  :ensure t)
```

### Manual Installation

Clone this repository and add it to your load path:

```elisp
(add-to-list 'load-path "/path/to/dprint.el")
(require 'dprint)
```

## Usage

Format the current buffer:

```
M-x dprint-prettify
```

You can bind this to a key for quick access:

```elisp
(global-set-key (kbd "C-c f") #'dprint-prettify)
```

## Configuration

dprint.el uses the standard dprint configuration file (`dprint.json` or `.dprint.json`) in your project root. Refer to the [dprint configuration documentation](https://dprint.dev/config/) for setup instructions.

## Related Projects

- [dprint](https://github.com/dprint/dprint) - The core formatter
- [dprint plugins](https://dprint.dev/plugins/) - Available formatting plugins

## License

This project is licensed under the GNU General Public License v3.0. See [LICENSE](LICENSE) for details.

## Author

Naoya Yamashita ([@conao3](https://github.com/conao3))
