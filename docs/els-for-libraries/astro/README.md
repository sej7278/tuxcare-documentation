# Astro

Endless Lifecycle Support (ELS) for Astro from TuxCare provides security fixes for Astro versions that have reached their end of life. This allows you to continue running Astro applications without vulnerability concerns, even after official support has ended.

## Supported Astro Versions

* Astro 0.26.1, 1.9.2, 2.10.15

## Connection to ELS for Astro Library

This guide outlines the steps needed to integrate the TuxCare ELS for the Astro library.

## Step 1: Get Token

You need a token in order to use TuxCare ELS Astro library. Anonymous access is disabled. To receive the token, please contact [sales@tuxcare.com](mailto:sales@tuxcare.com).

## Step 2: Set Up ELS for Astro

TuxCare provides ELS for Astro as an NPM package, hosted on a secure internal registry. Follow the steps below to add it to your project and get started.

1. Navigate to the root directory of your Astro project.
2. Create a `.npmrc` file or update it if it already exists.

   **Example:**

   ```text
   my-astro-project/
   ├── node_modules/
   ├── package.json
   ├── .npmrc         ⚠️ ← Create it here
   └── package-lock.json
   ```

3. Use an editor of your choice (e.g., VS Code) to add the following registry address line:

   ```text
   registry=https://registry.npmjs.org/
   @els-js:registry=https://nexus.repo.tuxcare.com/repository/els_js/
   //nexus.repo.tuxcare.com/repository/els_js/:_auth=${TOKEN}
   ```

   :::warning
   Replace ${TOKEN} with the token you received from [sales@tuxcare.com](mailto:sales@tuxcare.com).
   :::

4. Update your `package.json` file to replace your Astro dependencies with the TuxCare packages. Choose your Astro version below and add the `dependencies` and `overrides` entries shown.

    <TableTabs label="Choose Astro version: " >

    <template #astro_0.26.1>

    ```text
    "dependencies": {
      "astro": "npm:@els-js/astro@>=0.26.1-tuxcare.1"
    },
    "overrides": {
      "astro@0.26.1": "npm:@els-js/astro@>=0.26.1-tuxcare.1"
    }
    ```

    </template>

    <template #astro_1.9.2>

    ```text
    "dependencies": {
      "astro": "npm:@els-js/astro@>=1.9.2-tuxcare.1"
    },
    "overrides": {
      "astro@1.9.2": "npm:@els-js/astro@>=1.9.2-tuxcare.1"
    }
    ```

    </template>

    <template #astro_2.10.15>

    ```text
    "dependencies": {
      "astro": "npm:@els-js/astro@>=2.10.15-tuxcare.1"
    },
    "overrides": {
      "astro@2.10.15": "npm:@els-js/astro@>=2.10.15-tuxcare.1"
    }
    ```

    </template>

    </TableTabs>

5. You need to remove the `node_modules` directory and the `package-lock.json` file, and also clear the `npm cache` before installing the patched packages. Use the following commands:

   ```text
   rm -rf node_modules package-lock.json && npm cache clean --force
   ```

6. Run the following command to install the ELS version of the Astro library (token for the TuxCare repository will be automatically picked up from your `.npmrc` file):

   ```text
   npm install
   ```

## Step 3: Verify Installation

1. To confirm the TuxCare Astro library is set up correctly, use npm to list the project's dependencies:

   ```text
   npm list
   ```

2. After reviewing the dependencies, run your application to ensure everything works correctly.

The `npm` tool should be able to identify and resolve dependencies from the TuxCare ELS for Astro repository.

## Vulnerability Exploitability eXchange (VEX)

VEX is a machine-readable format that tells you if a known vulnerability is actually exploitable in your product. It reduces false positives, helps prioritize real risks.

TuxCare provides VEX for Astro ELS versions: [security.tuxcare.com/vex/cyclonedx/els_lang_javascript/astro/](https://security.tuxcare.com/vex/cyclonedx/els_lang_javascript/astro/).

## Software Bill of Materials (SBOM)

For each published ELS package and version, TuxCare generates SBOM files. Those artifacts are published to TuxCare Nexus.

You can browse SBOM files for Astro here:

[https://nexus.repo.tuxcare.com/#browse/browse:els-js-sbom:astro](https://nexus.repo.tuxcare.com/#browse/browse:els-js-sbom:astro)

Use the credentials you received for TuxCare ELS ([Step 1: Get Token](#step-1:-get-token)) to access Nexus.

## How to Upgrade to a Newer Version of TuxCare Packages

If you have already installed a package with a `tuxcare.1` suffix and want to upgrade to a newer release (for example, `tuxcare.3`), remove node_modules, clear the npm cache to avoid conflicts, and then run the installation command:

  ```text
  rm -rf node_modules package-lock.json && npm cache clean --force
  npm install
  ```

## Resolved CVEs

Fixes for the following vulnerabilities are available in ELS for Astro from TuxCare versions:

<TableTabs label="Choose Astro version: " >

<template #astro_0.26.1>

|     CVE ID     | CVE Type | Severity | Affected Libraries |      Vulnerable Versions       |
|:--------------:| :------: |:--------:|:------------------:|:------------------------------:|
| CVE-2024-56140 | Direct   | Medium   |       astro        |          < 4.16.17             |
| CVE-2024-56159 | Direct   | Medium   |       astro        | <= 4.16.17, >= 5.0.0 <= 5.0.8  |
| CVE-2025-55303 | Direct   | Medium   |       astro        | < 4.16.18, >= 5.0.0 < 5.13.2   |
| CVE-2025-61925 | Direct   | Medium   |       astro        |          < 5.14.2              |
| CVE-2025-64757 | Direct   | Low      |       astro        |          < 5.14.3              |
| CVE-2025-64764 | Direct   | Medium   |       astro        |          < 5.15.8              |
| CVE-2025-64765 | Direct   | Medium   |       astro        |          < 5.15.8              |
| CVE-2025-65019 | Direct   | Medium   |       astro        |          < 5.15.9              |
| CVE-2025-66202 | Direct   | Medium   |       astro        |          < 5.15.8              |
| CVE-2026-41067 | Direct   | Medium   |       astro        |          < 6.1.6               |

</template>

<template #astro_1.9.2>

|     CVE ID     | CVE Type | Severity | Affected Libraries |      Vulnerable Versions       |
|:--------------:| :------: |:--------:|:------------------:|:------------------------------:|
| CVE-2024-56140 | Direct   | Medium   |       astro        |          < 4.16.17             |
| CVE-2024-56159 | Direct   | Medium   |       astro        | <= 4.16.17, >= 5.0.0 <= 5.0.8  |
| CVE-2025-55303 | Direct   | Medium   |       astro        | < 4.16.18, >= 5.0.0 < 5.13.2   |
| CVE-2025-61925 | Direct   | Medium   |       astro        |          < 5.14.2              |
| CVE-2025-64757 | Direct   | Low      |       astro        |          < 5.14.3              |
| CVE-2025-64764 | Direct   | Medium   |       astro        |          < 5.15.8              |
| CVE-2025-64765 | Direct   | Medium   |       astro        |          < 5.15.8              |
| CVE-2025-65019 | Direct   | Medium   |       astro        |          < 5.15.9              |
| CVE-2025-66202 | Direct   | Medium   |       astro        |          < 5.15.8              |
| CVE-2026-41067 | Direct   | Medium   |       astro        |          < 6.1.6               |

</template>

<template #astro_2.10.15>

|     CVE ID     | CVE Type | Severity | Affected Libraries |      Vulnerable Versions       |
|:--------------:| :------: |:--------:|:------------------:|:------------------------------:|
| CVE-2024-56140 | Direct   | Medium   |       astro        |          < 4.16.17             |
| CVE-2024-56159 | Direct   | Medium   |       astro        | <= 4.16.17, >= 5.0.0 <= 5.0.8  |
| CVE-2025-55303 | Direct   | Medium   |       astro        | < 4.16.18, >= 5.0.0 < 5.13.2   |
| CVE-2025-61925 | Direct   | Medium   |       astro        |          < 5.14.2              |
| CVE-2025-64757 | Direct   | Low      |       astro        |          < 5.14.3              |
| CVE-2025-64764 | Direct   | Medium   |       astro        |          < 5.15.8              |
| CVE-2025-64765 | Direct   | Medium   |       astro        |          < 5.15.8              |
| CVE-2025-65019 | Direct   | Medium   |       astro        |          < 5.15.9              |
| CVE-2025-66202 | Direct   | Medium   |       astro        |          < 5.15.8              |
| CVE-2026-33769 | Direct   | Medium   |       astro        |     >= 2.10.10 < 5.18.1        |
| CVE-2026-41067 | Direct   | Medium   |       astro        |          < 6.1.6               |

</template>

</TableTabs>

If you are interested in the TuxCare Endless Lifecycle Support, contact [sales@tuxcare.com](mailto:sales@tuxcare.com).
