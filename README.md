
# 1. Specific Test II - OCR Techniques Evaluated:
Three OCR methods were tested to extract text from the manuscript:
- PaddleOCR (CNN, RNN, Transformer-based) – Selected for its multi-language support, fast inference, and superior accuracy.
- Tesseract OCR (CRNN + CTC Loss) – Used with Spanish language support but potentially less effective for complex layouts.
- EasyOCR (VGG + LSTM + CTC Loss) – Another deep learning-based OCR alternative.

The Character Error Rate (CER) and Word Error Rate (WER) were used to evaluate the accuracy of each OCR output against the ground truth text.

# 2. Specific Test I - Layout Recognition Techniques:
- Two layout recognition methods were tested to detect text regions:
- U-Net based segmentation model – A CNN-based encoder-decoder approach for text layout detection.
- Canny edge detection with contour filtering – Utilized to identify tightly packed text regions using edge detection and morphological operations.

# 3. OCR + Layout Detection Integration:
PaddleOCR was integrated with bounding boxes to visualize detected text areas on the manuscript image.

Outcome:
- PaddleOCR demonstrated the highest accuracy and adaptability for Spanish text.
- Layout recognition models improved text localization, resulting in more structured OCR outputs.
- Evaluation metrics (CER, WER) provided quantitative insights into OCR performance.
