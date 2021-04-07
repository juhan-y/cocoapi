COCO 데이터셋: coco dataset은 object dectection, segmentation, captioning하는 데이터셋인데 여러 가지의 class가 존재한다. COCO dataset은 kitti dataset과 비슷하게 전반적인 이미지를 dataset으로 갖고 있다. 다른점은 COCO dataset은 도로상황이나 차량이 아닌 전반적인 다양한 이미지들을 가지고 있으며, 그에 따른 label의 class도 상당히 다양하다.
yolov3와 같이 object detection을 위한 deep neural network model을 만드는데 자주 사용되고 실제로 yolov3논문을 살펴보면 COCO dataset으로 detector(model)의 성능을 평가하였다.(mAP) COCO 데이터셋의 labelling도 kitti 데이터셋과 비슷하게 객체에 대한 정보를 txt파일에 저장하게 되는데 kitti dataset과 다르게 단순한 바운딩박스로 이루어진 사각형으로 객체를 특정하는 것이 아니라 segmentation과 같이 객체의 경계선상으로 특정하게된다. 또 다른점은 kitti dataset의 txt파일내부 요소의 개수가 16개인데 반해 COCO dataset은 class만 91개로 엄청나게 많은 class개수를 가지고 있다.(실제로 사용되는 class개수는 80개) 좀 더 보편적인 이미지에 대한 라벨링이 되어있는 것을 알 수 있다.
image의 개수는 330,000개 가량 있고 그 중 라벨링이 된 개수는 200,000개가 넘는다고 한다. COCO dataset 홈페이지에 들어가보면 매년마다 새로운 규칙으로 과제가 있어서 그 과제에 대한 평가와 수여식이 있다고 한다. git에 첨부한 COCO dataset tutorial은 COCO dataset에 관한 파이썬과 매트랩, Lua를 이용하여 tutorial을 진행할 수 있게 코드가 작성된 API파일들과 yml파일 등이 있다.
활용분야는 자율주행에 있어서도 가능하고 일반적인 카메라로 활용될 수 있는 분야에서는 다양하게 이용될 수 있다.

<COCO dataset image에 labelling이 되어있는 모습을 나타낸 image>

