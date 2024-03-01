# Testing OCR in Azure
In this project, I used the Optical Character Recognition service available in Azure to test the accuracy of the text-extraction capabilities of the AI product. In order to do so, I sourced (unrestricted) images from the internet which had something written on them.

### Image #1

The first image was read well by Azure. The words it couldn't make out were mostly too small and hard to read due to the resolution in such dimensions. It had some trouble making out that different words were different words and not a clump of characters sticked together. In general it was surprising by being able to accurately read words in different orientations, as some were written horizontally and other vertically.

### Image #2

The second image had similar results to the first one. Also had some trouble making out different words and some characters were incorrectly interpreted, presumable due to the handwriting-like font present in the photo.

### Image #3

The third image had the worst performance. Azure was unable to correctly read many of the words, though this is expected due to the low resolution image with bad handwriting.

### Conclusion

The takeaway is that the OCR service in Azure is a fast, mostly accurate way to process text in images. It is not perfectly accurate, which means further adjustments may be needed in the case of images which are not ideal for reading text.