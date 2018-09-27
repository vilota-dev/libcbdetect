Libdetect
---
Unofficial implemention of [libcbdetect](http://www.cvlibs.net/software/libcbdetect/) in C++.  
  
Libdetect is a fully automatic sub-pixel checkerboard / chessboard pattern detection. The algorithm autmatically extracts corners to sub-pixel accuracy and combines them to (rectangular) checkerboards / chessboard-like patterns.  
  
#### Require
- C++ 11  
- Opencv >= 3.0  
  
#### Example
> using namespace cbdetect;  
> cv::Mat img = cv::imread("image.bmp", cv::IMREAD_GRAYSCALE);  
> find_corners(img, 0.01, corners);  
> plot_corners(img, corners);  
> chessboards_from_corners(corners, chessboards);  
> plot_chessboards(img, corners, chessboards);

    
#### Reference Papers
[1]  Andreas Geiger and Frank Moosmann and Oemer Car and Bernhard Schuster, Automatic Calibration of Range and Camera Sensors using a single Shot, ICRA, 2012  
[2] Miriam Schoenbein and Tobias Strauss and Andreas Geiger, Calibrating and Centering Quasi-Central Catadioptric Cameras, ICRA, 2014  
