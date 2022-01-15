# Image Sort by Saturation

## Description
This package is designed to run on Google Colab and will sort Google Drive photos into color and grayscale categories.

## Rules for Usage
This tool is open-source and free for you to use, duplicate, and modify. If you do, please acknowledge the original author, [James Swartwood](https://github.com/jamesswartwood), however you feel is appropriate for your situation. Thank you!

## Quick Start Guide
- Clone this repository to your Google Drive
    - Create a new Colab document
    - Run this block of code (feel free to update the `cd` path to point to a different location in your Google Drive):
    ```
    from google.colab import drive
    drive.mount('/content/gdrive')
    %cd gdrive/My Drive
    !git clone https://github.com/jamesswartwood/image-sort-by-saturation.git
    ```
- Navigate to the cloned folder and open `image_sort.ipynb`
- Update the settings in the `Configure Progam Settings` section to your desired preferences
- Run all blocks of code sequentially
- Check to make sure that the program organized the images as you intended

## Tips
- This tool operates by finding the average saturation (color value) of each image and compares them to the indicated threshold. This method is not without flaws. The program functions best when operating on similar photos, such as camera trap images from a single camera.
- To find the threshold that will work best for you, use `threshold_finder.ipynb` and follow the instructions included in the document.

## Planned Features
- An automatic threshold finder for a subset of labeled images
- Deeper analysis of image features for better results

## Support
Contact the author of this code, [James Swartwood](https://github.com/jamesswartwood), if you have any issues, questions, or suggestions.
