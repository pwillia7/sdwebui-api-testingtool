# Testing Tool Script

## Description
This script processes a CSV file containing image URLs and prompts to generate images via an API call and combines them with labels into a montage.

## Requirements
- Python 3.x
- Requests library
- Pillow library
- An API endpoint for image generation

## Usage
To use this script, you must have a CSV file named `input.csv` with columns `URL` and `Prompt`. Optionally, you can pass a title for the test as a command line argument, which will be included in the montage and the folder name.

### Command Line Syntax
```bash
python testingtool.py [title]
```
Where [title] is an optional title for the test.

## CSV File Format
The `input.csv` should follow this format:

```csv
URL,Prompt
http://example.com/image1.jpg,"Generate an image based on this prompt"
http://example.com/image2.jpg,"Another prompt for image generation"
```
## Output
The script will create a timestamped folder (optionally prefixed with the title) containing all original and generated images and a combined montage image named `combined_output.jpg`.

## Troubleshooting
Ensure the API endpoint is correctly set and accessible. Adjust the script parameters as needed for your environment and API specifications.


