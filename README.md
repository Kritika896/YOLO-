OBJECT DETECTION USING YOLO

How YOLO Works (You Only Look Once)
YOLO is a real-time object detection model that processes an image in one pass through the neural network, making it fast and efficient.
Working of YOLO
1.	Image Input
o	The input image is resized and passed into the YOLO model.
o	Example: A 640×640 image is fed into the model.
2.	Grid Division & Feature Extraction
o	The image is divided into S×S grid cells (e.g., 13×13 or 19×19).
o	Each cell is responsible for detecting objects if the object’s center falls inside that cell.
3.	Bounding Box Predictions
o	Each cell predicts multiple bounding boxes, along with:
	(x, y) → Center coordinates of the object.
	(w, h) → Width and height of the bounding box.
	Confidence Score → Probability that an object is present in the box.
4.	Class Predictions
o	Each detected object is classified into predefined categories (e.g., dog, car, person).
5.	Non-Maximum Suppression (NMS)
o	Removes duplicate and overlapping bounding boxes, keeping the one with the highest confidence score.
6.	Final Output
o	The model outputs bounding boxes, class labels, and confidence scores.
o	The detected objects are displayed and saved.
