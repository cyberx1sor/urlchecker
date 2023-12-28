# Clean URLs and Verify Status Codes

This Bash script cleans URLs from an input file and verifies their status codes using cURL. Cleaned URLs and their status codes are stored in an output file.

## Usage

```bash
chmod +x urlchecker
./urlchecker <input_file> -o <output_file>
```
<input_file>: File containing the URLs to clean and verify.

<output_file>: Output file where valid URLs and their status codes will be saved.

## Example
```bash
./urlchecker urls.txt -o valid_urls.txt
```

This command will clean the URLs from the urls.txt file and save valid URLs along with their status codes in valid_urls.txt.

## Recommendation (but not required)

Copy the file urlchecker in your Linux path /usr/bin/urlchcker with sudo.

Make sure to launch this command first to make the file executable: ```sudo chmod +x /usr/bin/urlchecker```

This way, you will be able to launch urlchecker regardless of the directory you are in.

## Features

Cleans URLs by removing additional text after the domain.

Verifies the status code of each URL using cURL.

Displays the result in colors in the terminal.

Saves valid URLs and their status codes in an output file.


## Requirements
Bash

cURL
