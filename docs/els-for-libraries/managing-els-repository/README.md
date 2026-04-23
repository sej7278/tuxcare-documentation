# Managing the ELS repository

This page provides instructions for upgrading to newer TuxCare package versions and accessing source code for ELS-patched libraries.

## Upgrading to a newer TuxCare version

To update to a newer TuxCare-patched release, follow the instructions for your ecosystem.

### Java libraries

<TableTabs label="Choose library: ">

<template #Apache_Commons_Lang>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Apache_CXF>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Apache_Kafka>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Apache_Log4j>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Apache_Lucene_and_Solr>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Apache_Spark>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Apache_Struts>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Apache_Tomcat>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Apache_Velocity_Engine>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Hibernate>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Jackson>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Jetty>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #PostgreSQL_Driver>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Protobuf>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version strings in your Maven or Gradle build file.

</template>

<template #Spring>

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), update the version string in your Maven or Gradle build file.

</template>

</TableTabs>

### PHP libraries

<TableTabs label="Choose library: ">

<template #AWS_SDK_for_PHP>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require aws/aws-sdk-php:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #Browsershot>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require spatie/browsershot:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #CakePHP>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require cakephp/cakephp:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #Carbon>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require nesbot/carbon:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #CraftCMS>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require craftcms/cms:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #CraftCMS_Feed_Me>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require craftcms/feed-me:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #Dompdf>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require dompdf/dompdf:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #Firebase_PHP_JWT>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require firebase/php-jwt:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #Laravel>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require laravel/framework:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #League_CommonMark>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require league/commonmark:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #Livewire>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require livewire/livewire:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #PHP_SVG_Lib>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require phenx/php-svg-lib:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #PHPMailer>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require phpmailer/phpmailer:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #PhpSpreadsheet>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require phpoffice/phpspreadsheet:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #PHPUnit>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require sebastianbergmann/phpunit:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #SwiftMailer>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require swiftmailer/swiftmailer:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #Symfony>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require symfony/process:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

<template #Zend_Framework>

Update the version string in your `composer.json` file or run the `composer require` command with the new version:

```text
composer require zendframework/zendframework1:VERSION-pN+tuxcare
```

Then run `composer update` to apply the changes:

```text
composer update
```

</template>

</TableTabs>

### Python libraries

To upgrade to a newer TuxCare release (e.g., from `version.post1+tuxcare` to `version.post2+tuxcare`), use the same installation method you used during setup and specify the newer package version.

### JavaScript libraries

To upgrade to a newer TuxCare release (for example, from `tuxcare.1` to `tuxcare.3`), remove `node_modules`, clear the npm cache to avoid conflicts, and then run the installation command:

```text
rm -rf node_modules package-lock.json && npm cache clean --force
npm install
```

## Source code

TuxCare provides source code for patched applications in the [Nexus repository](https://nexus.repo.tuxcare.com/#browse/browse). Source archives and JARs follow the standard naming conventions with a `-sources` classifier or suffix.

:::tip
If a source archive is not available for a specific package, please contact [sales@tuxcare.com](mailto:sales@tuxcare.com).
:::
