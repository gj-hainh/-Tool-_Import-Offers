
# Import Offers Tool

`import-offers` is a tool designed to facilitate the batch import of offers into a system using a CSV file. It can be used for testing, experimentation, and development during software development.

## System Requirements

To install and use this tool, your system needs to have `nodejs version v14.16.0` or higher and `npm version 6.14.11` or higher.

## Installation

To install this tool, please download the `import-offers-1.0.0.tgz` file from the provided source and run the following command in the folder containing the downloaded file:

```
npm install -g import-offers-1.0.0.tgz
```

You can verify that the installation was successful by running the command:

```
import-offers --version
```

## Usage

To use this tool, you can refer to the command `import-offers --help` to view a list of supported parameters.

The current available parameters in version 1.0.0 are as follows:

- `--endpoint` (required): The API URL Endpoint to use to import an offer into the system. This will be provided by the developer.
- `--filePath` (required): The path to the CSV file containing the list of offers to be imported.
- `--logsLevel` (optional): Specify the level of logs to export to the console, including error, success, all.
- `--outDir` (optional): The directory to export the report file.

### Sample Command

Here is an example command you can use to import offers:

```
import-offers --endpoint [[provided by the developer] --filePath offer_ids.csv --logsLevel error --outDir Desktop
```

This tool is very useful for simulating the offer importing process on production. You can use it to test and experiment before deploying to production to ensure the system's stability and performance.
