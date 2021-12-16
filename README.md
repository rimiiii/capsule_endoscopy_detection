# capsule_endoscopy_detection
[DACON] 병변 검출 AI 경진 대회

# Label 형태
class, 0과 1 사이로 scaling된 x center, y center, weight, height

# yaml 파일 형태
- dir: path/to/imgs
  ```
  path: ../datasets/VisDrone  # dataset root dir
  train: VisDrone2019-DET-train/images  # train images (relative to 'path')  6471 images
  val: VisDrone2019-DET-val/images  # val images (relative to 'path')  548 images
  test: VisDrone2019-DET-test-dev/images  # test images (optional)  1610 images
  ```
- file: path/to/imgs.txt
    
    ```python
    path: ../datasets/coco  # dataset root dir
    train: train2017.txt  # train images (relative to 'path') 118287 images
    val: val2017.txt  # train images (relative to 'path') 5000 images
    test: test-dev2017.txt  # 20288 of 40670 images, submit to https://competitions.codalab.org/competitions/20794
    ```
- list:[path/to/imgs1, path/to/imgs2..]
    
    ```python
    path: ../datasets/GlobalWheat2020  # dataset root dir
    train: # train images (relative to 'path') 3422 images
      - images/arvalis_1
      - images/arvalis_2
      - images/arvalis_3
      - images/ethz_1
      - images/rres_1
      - images/inrae_1
      - images/usask_1
    val: # val images (relative to 'path') 748 images (WARNING: train set contains ethz_1)
      - images/ethz_1
    test: # test images (optional) 1276 images
      - images/utokyo_1
      - images/utokyo_2
      - images/nau_1
      - images/uq_1
    ```
