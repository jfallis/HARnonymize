# HARnonymize

HARnonymize is a tool designed to provide secure and reliable anonymization of HTTP Archive (HAR) files. HARnonymize anonymize HAR files by removing sensitive information such as cookies, passwords, and other personally identifiable information (PII). 

This software is designed to ensure that sensitive information included in HAR files is kept confidential and protected from unauthorized access. 

## How to use

The `HARnonymize.zip` zipped file contains pre-compiled binaries for three major operating systems: Windows, Linux, and Mac OS X. These binaries are ready to use, eliminating the need for users to compile the source code before running the application.

- Windows: `harnonymize-windows.exe`
- Linux: `harnonymize-linux`
- Mac OS X (Before 2020 laptops): `harnonymize-amd64-macos`
- Mac OS X (Latest laptops): `harnonymize-arm64-macos`

To use the tool, first download the [zipped file](https://raw.githubusercontent.com/jfallis/HARnonymize/main/HARnonymize.zip). 

The keywords in the block.txt file are not case-sensitive. It is crucial to add any additional keywords that should be blocked, separated by new lines.

Example block.txt file:
```text
secure id
password
john fallis
sensitive information
```

Next, drag and drop the exported HAR files into the directory where the binary is located. 
Then, run the binary. The application will automatically process all HAR files in the directory. 
After processing, anonymized HAR files will be generated with the same name as the original HAR files, but with the prefix `anonymized_`.