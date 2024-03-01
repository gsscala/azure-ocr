# Testing OCR in Azure
In this project, I used the Optical Character Recognition service available in Azure to test the accuracy of the text-extraction capabilities of the AI product. In order to do so, I sourced (unrestricted) images from the internet which had something written on them.
|Image #1|Image #2|Image #3|
|---|---|---|
|![Image1](https://raw.githubusercontent.com/gsscala/azure-ocr/main/input/image-1.jpg)|![Image2](https://raw.githubusercontent.com/gsscala/azure-ocr/main/input/image-2.png)|![Image3](https://raw.githubusercontent.com/gsscala/azure-ocr/main/input/image-3.jpg)|
|The first image was read well by Azure. The words it couldn't make out were mostly too small and hard to read due to the resolution in such dimensions. It had some trouble making out that different words were different words and not a clump of characters sticked together. In general it was surprising by being able to accurately read words in different orientations, as some were written horizontally and other vertically.|The second image had similar results to the first one. Also had some trouble making out different words and some characters were incorrectly interpreted, presumable due to the handwriting-like font present in the photo.|The third image had the worst performance. Azure was unable to correctly read many of the words, though this is expected due to the low resolution image with bad handwriting.|

### Conclusion

The takeaway is that the OCR service in Azure is a fast, mostly accurate way to process text in images. It is not perfectly reliable, which means further adjustments may be needed in the case of images which are not ideal for reading text, such as the third example.
