# 放电检测

#### Description
• Use QT to develop discharge analysis software that can run on the win/linux platform, organize the algorithm modules according to the strategy mode, and quickly perform the migration verification of the algorithm modules;

• Use OpenCV to complete the collection and initialization of the data in the discharge video; perform video processing for the imported video, and use the frame difference method to realize the separation of the foreground and the background;

• For the foreground, complete image binarization, discharge area detection, extraction, and statistics, and use the background moving average method to overcome the abnormalities caused by the lens shake of some UV cameras.

#### Software Architecture
Strategy pattern organization algorithm module

Multi-thread scheduling completes video stream processing and discharge intensity curve update

#### Installation

1.  git clone https://gitee.com/dagunliyu/discharge-detection.git 

#### Instructions

1.  Import the discharge video stream taken by the UV camera
2. Automatically perform playback and discharge intensity statistics
3. After the video stream processing is over, the statistical discharge intensity, rate of change and other information can be exported through excel

#### Contribution

1.  @Yang provides discharge video


#### Gitee Feature

1.  Application of Strategy Pattern
2. Frame difference method to extract the discharge foreground
3. Background moving average overcomes video jitter
4. Count the top three discharge areas of discharge intensity, use bbox to mark and mark the number of pixels
5. Count and mark the pixels of the discharge area
6. Count the change rate of pixels in the discharge area
7. The discharge intensity, rate of change and other information are exported through excel
8. Import current and voltage data and display
9. The XY axis of the curve can be zoomed and dragged, and the curve can be moved as a whole
