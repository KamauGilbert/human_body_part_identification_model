## Human Body Part Identification Model


This is a computer vision model designed to identify 17 parts of the human body. The parts are:

- bm_arm_left
- bm_arm_right
- bm_body_up
- bm_hand_left
- bm_hand_right
- bm_head
- bm_leftfoot
- bm_leftknee
- bm_leftleg
- bm_leftsleg
- bm_neck
- bm_rightfoot
- bm_rightknee
- bm_rightleg
- bm_rightsleg
- bm_sarm_left
- bm_sarm_right

### Dataset

- Find the dataset [here](https://universe.roboflow.com/irtzm/person_part_seg_bm/dataset/5).
- [Roboflow](https://universe.roboflow.com/) offers various image datasets for deep learning, including object detection, classification, semantic segmentation, instance segmentation, and keypoint detection datasets.

### Purpose of the Model

- **Emergency Response**: The model aims to assist emergency response units by identifying body parts to detect injuries.
- **Injury Detection**: Plans to combine this dataset with an 'Injury Dataset' to detect and identify the type and location of injuries on a person.

### Training and Testing

- **Current Status** (As of 17th May 2024):
  - Trained using YOLOv8 and Detectron2.
  - Initial training and tests with YOLOv8 showed low accuracy (e.g., bm_body_up was identified as bm_head).
  - Low accuracy may be due to:
    - Limited dataset (318 images).
    - Low number of epochs (100).
      
  - I managed to train and test the Detectron2 model.Detectron2 offered a better output compared to YOLOv8. Find the Detectron2 output image under the detectron model test output png image.
  
- **Future Plans**:
  - Augment dataset.
  - Increase the number of epochs used on YOLOv8 during training.
  - Re-test to improve accuracy.

### Challenges

- **Limited Data**: Training on only 318 images.
- **Computational Limits**: Colab deactivated GPU during Detectron2 testing.

### Next Steps

- Train and test the model with augmented data and more epochs.
- Compare the performance of YOLOv8 and Detectron2.
- Update this README with results and improvements.

