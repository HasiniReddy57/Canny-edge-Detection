The project Canny Edge Detector is designed as an embedded system model in SystemC suitable for SoC implementation.

## Objective 
To develop an efficient edge detection algorithm that accurately identifies edges in images using the principles of the Canny edge detection method.

## Key Components

Gaussian Smoothing: Reduces noise in the input image to prepare for gradient calculation.
Gradient Computation: Calculates the gradient in both the x and y directions to identify the intensity of edges.
Magnitude and Direction: Determines the strength and direction of edges using the calculated gradients.
Non-Maximum Suppression: Refines edge detection by eliminating non-maximum responses, enhancing the accuracy of edge localization.
Hysteresis Thresholding: Applies dual thresholds to distinguish strong edges from weak ones, allowing for continuous edge tracing.
Modular Design: Each stage of the edge detection process is encapsulated in separate SystemC modules, ensuring a clean, organized architecture that allows for easy testing and modifications.

## Data Flow
Utilizes sc_fifo channels for efficient inter-module communication, ensuring smooth data transfer and maintaining real-time processing capabilities.

## Flexibility
The algorithm supports adjustable high and low threshold values, enabling fine-tuning based on specific application requirements.

## Performance
Designed for speed and accuracy, the system successfully identifies and preserves edges while minimizing the impact of noise and false positives.

## Results
Demonstrated high-quality edge detection in various test images, with clear delineation of edges, making it suitable for applications in image processing and computer vision tasks.
