# DynamoDbExportCsv

A simple library / CLI tool for exporting a dynamodb table to a CSV file

## Installation

### CLI tool
``` bash
  $ [sudo] npm install DynamoDBExportCSV -g
```

### Library
``` bash
  $ npm install DynamoDBExportCSV --save
```

## Usage
``` bash
  $ ./bin/DynamoDBExportCSV --awsregion "us-west-2" --awsid "id" --awssecret "secret" --table "mytable" --columns "columna,columnb,columnc" --gzip
```

This will create a sub directory in the current working directory with the same name as the table.  The csv files
will be compressed with gzip.

Parallel Scans are useful to maximize usage of throughput provisioned on the DynamoDb table.