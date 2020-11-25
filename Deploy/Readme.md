# Face-Detection-Lite(Under Construction)
Smart_V0-V4 are lightweight face detection models designed for a project in SmartSens.
All models use MobileNetV2[1] as backbone and relu as activation function(with out deformable convolution).

# About SmartSens
SmartSens Technology Co., Ltd. is a high-performance CMOS image sensing (CIS) chip design company. The company, founded in 2011, is headquartered in Shanghai and has both research centers and sales offices in various cities around the world, including Beijing, Shenzhen, Hangzhou, Hong Kong, Hsinchu and San Jose, California.

# Comparison with other lightweight face detection models
| Style | MAdds | Parameters | easy | medium | hard |
|:-|:-:|:-:|:-:|:-:|:-:|
| Smart_V0 | 0.27B | 0.10M | 84.9% | 81.4% | 64.0% |
| |
| Smart_V1(640) | 0.67B | 0.27M | 89.8% | 84.9% | 53.8% |
| Ultra_1M_RBF(640)[2] |   | ~0.3M | 85.5% | 82.2% | 57.9% |
| libfacedetection_v2(640)[3] |  | 0.8M | 77.3% | 71.8% | 48.5% |
| |
| Smart_V1 | 0.67B | 0.27M | 91.0% | 88.8% | 75.4% |
| ASFD_D0[4] | 0.73B | 0.62M | 90.1% | 87.5% | 74.4% |
| |
| Smart_V2 | 1.1B | 0.48M | 92.8% | 90.9% | 79.4% |
| CenterFace[5] |  | 1.8M | 92.2% | 91.1% | 78.2% |
| RetinaFace_Ori[6] | 1.0B | 0.44M | 89.6% | 87.1% | 69.1% |
| RetinaFace_biubug6[7] | 1.0B | 0.44M | 90.7% | 88.2% | 73.8% |
| |
| Smart_V3 | 1.17B | 0.59M | 93.3% | 91.5% | 80.5% |
| RetinaFace_libin(DCN)[8] |  | 0.65M | 92.7% | 90.9% | 80.2% |
| |
| Smart_V4 | 3.89B | 2.26M | 93.9% | 92.9% | 83.7% |
| ASFD_D1[4] | 4.27B | 3.9M | 93.3% | 91.7% | 83.6% |
* (640) uses VGA 640*480 or scaling by the maximum side length of 640 as input. 
* The other evaluations use Single Inference on the Original Scale.

# Dependencies
* numpy
* opencv
* onnxruntime(pip install onnxruntime)

# Run Demo
python test_image.py
