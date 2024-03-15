# charonlab/static-analysis

[![PHP Version Require](https://poser.pugx.org/charonlab/static-analysis/require/php)](https://packagist.org/packages/charonlab/static-analysis)
[![Latest Stable Version](https://poser.pugx.org/charonlab/static-analysis/v/stable)](https://packagist.org/packages/charonlab/static-analysis)
[![Total Downloads](https://poser.pugx.org/charonlab/static-analysis/downloads)](https://packagist.org/charonlab/static-analysis)
[![License](https://poser.pugx.org/charonlab/static-analysis/license.svg)](https://packagist.org/packages/charonlab/static-analysis)


## Installation

Use the composer to install:

```bash
composer require --dev charonlab/static-analysis
```

## Usage

#### Psalm

Create a `psalm.xml` file, below is a sample configuration.

```xml
<?xml version="1.0"?>
<psalm xmlns="https://getpsalm.org/schema/config"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="https://getpsalm.org/schema/config vendor/vimeo/psalm/config.xsd"
       errorLevel="2"
       hoistConstants="true"
       findUnusedPsalmSuppress="true"
       findUnusedVariablesAndParams="true"
       ensureArrayStringOffsetsExist="true"
       addParamDefaultToDocblockType="true"
       findUnusedBaselineEntry="true"
       findUnusedCode="false"
>
    <projectFiles>
        <directory name="src"/>
        <ignoreFiles>
            <directory name=".github"/>
            <directory name="vendor"/>
        </ignoreFiles>
    </projectFiles>
</psalm>
```

## Support

- [Issues](https://github.com/charonlab/static-analysis/issues/)

## License

The MIT License (MIT). Please see [License](LICENSE) for more information.
