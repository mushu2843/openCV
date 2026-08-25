# openCV
Performing some openCV Tasks usinG Google Colab


# Lab - 3
Object Detection: Finding what is in an image and where it is. Instead of just saying "there is a dog in this picture," it pinpoints the exact location of every object.
YOLO (You Only Look Once): A fast object detection algorithm. Older models scanned an image piece-by-piece multiple times, but YOLO looks at the entire image in a single pass to predict all objects instantly, making it ideal for real-time video.
YOLO and Deep Learning: YOLO is powered by a Convolutional Neural Network (CNN)—a deep learning model trained on millions of images to automatically recognize patterns like edges, shapes, textures, and full objects.
Bounding Boxes: The rectangular frames drawn around detected objects. They are defined by simple coordinates: center position $(x, y)$, width $(w)$, and height $(h)$.
Classification: Identifying the category or label of the object inside a bounding box (for example: car, person, traffic light, or dog).
Confidence Score: A number between 0 and 1 (or 0% to 100%) that tells you how certain the model is that an object exists in that box and belongs to that specific class.
IoU & Non-Maximum Suppression (NMS):IoU (Intersection over Union): Measures how much two bounding boxes overlap.Non-Maximum Suppression (NMS): YOLO often predicts multiple overlapping boxes for the same single object. NMS cleans up the clutter by keeping only the box with the highest confidence score and deleting the overlapping duplicates.
Training YOLO: Showing the model thousands of labeled images (images with manually drawn boxes and class tags). When YOLO makes a wrong guess, an optimization algorithm adjusts its internal neural weights until its predictions match the real ground-truth labels.
