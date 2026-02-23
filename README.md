# Background-Estimation-Motion-Detection-using-Differential-Motion-Analysis-using-Python

This project focuses on implementing a complete motion detection pipeline by combining background modeling using median filtering with frame-based differential motion analysis. The objective is to extract a stable background model from a grayscale video and detect moving objects by comparing each frame to the estimated background.

1. Background Estimation (Median Filtering)

Constructed a static background model from a grayscale video sequence.

The background was estimated by applying median filtering across the temporal dimension of the video. For each pixel location, the median intensity value across all frames was computed. This approach effectively removes moving objects and preserves stationary elements, producing a clean representation of the scene’s background.

Median filtering was chosen because it is robust to outliers, meaning transient moving objects do not significantly affect the background model.

2. Motion Detection (Differential Motion Analysis)

Each frame of the video was compared to the estimated background image using frame differencing

This produces a binary motion mask for each frame, clearly separating dynamic objects from static background regions.

This project demonstrates a foundational computer vision approach for motion detection, emphasizing robust background estimation and efficient pixel-wise motion analysis.
