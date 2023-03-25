This is a repository containing the Pytorch Implementations of the Popular Computer Vision Models
1. LeNet5 
2. AlexNet
3. VGG16
4. GoogLeNet(InceptionV1)
5. ResNet50


References: 
1. Y. Lecun, L. Bottou, Y. Bengio, and P. Haffner, “Gradient-Based Learning Applied to Document Recogni-
tion,” Proceedings of the IEEE 86 (11): 2278–2324, http://yann.lecun.com/exdb/publis/pdf/lecun-01a.pdf.

2. Alex Krizhevsky, Ilya Sutskever, and Geoffrey E. Hinton, “ImageNet Classification with Deep Convolutional
Neural Networks,” Communications of the ACM 60 (6): 84–90, https://dl.acm.org/doi/10.1145/3065386.

3. Karen Simonyan and Andrew Zisserman, “Very Deep Convolutional Networks for Large-Scale Image Recog-
nition,” 2014, https://arxiv.org/pdf/1409.1556v6.pdf.

4. Christian Szegedy, Christian, Wei Liu, Yangqing Jia, Pierre Sermanet, Scott Reed, Dragomir Anguelov, Dumi-
tru Erhan, Vincent Vanhoucke, and Andrew Rabinovich, “Going Deeper with Convolutions,” in Proceedings of
the IEEE Conference on Computer Vision and Pattern Recognition, 1–9, 2015, http://mng.bz/YryB.

5. Kaiming He, Xiangyu Zhang, Shaoqing Ren, and Jian Sun, “Deep Residual Learning for Image Recognition,”
2015, http://arxiv.org/abs/1512.03385.

Top-1 and top-5 error rates?
Top-1 and top-5 are terms used mostly in research papers to describe the accuracy
of an algorithm on a given classification task. The top-1 error rate is the percentage
of the time that the classifier did not give the correct class the highest score, and the
top-5 error rate is the percentage of the time that the classifier did not include the
correct class among its top five guesses.

AlexNet performance
AlexNet significantly outperformed all the prior competitors in the 2012 ILSVRC
challenges. It achieved a winning top-5 test error rate of 15.3%, compared to 26.2%
achieved by the second-best entry that year, which used other traditional classifiers.
This huge improvement in performance attracted the CV community’s attention to
the potential that convolutional networks have to solve complex vision problems and
led to more advanced CNN architectures, as you will see in the following sections of
this chapter.

VGG16 performance
VGG16 achieved a top-5 error rate of 8.1% on the ImageNet dataset compared to
15.3% achieved by AlexNet. VGG19 did even better: it was able to achieve a top-5
error rate of ~7.4%. It is worth noting that in spite of the larger number of parameters
and the greater depth of VGGNet compared to AlexNet, VGGNet required fewer
epochs to converge due to the implicit regularization imposed by greater depth and
smaller convolutional filter sizes.

Inception performance on the CIFAR dataset
GoogLeNet was the winner of the ILSVRC 2014 competition. It achieved a top-5 error
rate of 6.67%, which was very close to human-level performance and much better
than previous CNNs like AlexNet and VGGNet.

ResNet performance on the CIFAR dataset
The performance of ResNet models is benchmarked based on their results in the ILSVRC competition. ResNet-152
won first place in the 2015 classification competition with a top-5 error rate of 4.49%
with a single model and 3.57% using an ensemble of models. This was much better
than all the other networks, such as GoogLeNet (Inception), which achieved a top-5
error rate of 6.67%. ResNet also won first place in many object detection and image
localization challenges, as we will see in chapter 7. More importantly, the residual
blocks concept in ResNet opened the door to new possibilities for efficiently training
super-deep neural networks with hundreds of layers.

This models can be accessed from the torchvision.models package


