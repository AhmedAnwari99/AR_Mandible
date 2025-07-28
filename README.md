Computer Vision For Screen rendered Augmented Reality For Mandibular Tumor Surgery

Data:

2D Ct Scan projections + Live Video feed



Pipeline:

Manual Landmark Selection on both inputs.
Correspondence established -> Registration via RANSAC
Homography calculated and used to transform CT Scan.
Transformed CT projected over video. 
CT contains osteotomy path. Projected Osteotomy used to draw path on static camera frame.
Osteotomy drawn on static frame is used as guide to draw osteotomy path on actual object.
Validation done by surgeon.
Tracking via Optical Flow.

Semi-Automation via YOLOv8s.
Annotation via Label studio -> Ultralytics YOLOv8s model trained -> Detected landmarks used as points from Camera frame. CT Lnadmarks manually selected.


