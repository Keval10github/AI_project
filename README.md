# Vehicle Detection
> Vehicle Detection Using Deep Learning and YOLO Algorithm.


*(Train YOLO v5 on a Custom Dataset)*


<p float="center">
  <img src="https://user-images.githubusercontent.com/72157067/156183131-b661ba59-22e5-4c73-b5a9-e0b0855cc68a.jpg" width="600" />
  <img src="https://user-images.githubusercontent.com/72157067/156183111-cb0f09bb-cfe1-490f-bccc-335748111107.jpg" width="600" /> 
</p>

## Dataset

take or find vehicle images for create a special dataset for fine-tuning.

Train : 70%

Validition : 20%

Test : 10%


## Clone Vehicle-Detection Repository
```
cd Vehicle-Detection
pip install -r requirements.txt
```

## wandb

to have mAP, loss, confusion matrix, and other metrics, sign in www.wandb.ai.

```
pip install wandb
```

## Train

fine-tuning on a pre-trained model of yolov5.

```
python train.py --img 640 --batch 16 --epochs 50 --data dataset.yaml --weights yolov5m.pt
```

## Test

after train, gives you weights of train and you should use them for test.

```
python detect.py --weights runs/train/exp12/weights/best.pt --source test_images/imtest13.JPG
```


you can also use the weight file in path 'runs/train/exp12/weights/best.pt' without the train.
this weight is the result of 128 epoch train on the following dataset.

## My Vehicle Dataset
```
https://b2n.ir/vehicleDataset
```
## Team Members
```
1. Keval Ravani
2. Parthvi Rathod
3. Jay Rajodiya
4. Sneha Ramudu
5. Yashasvi Jain
```
