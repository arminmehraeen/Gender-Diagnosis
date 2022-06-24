# Gender-Diagnosis
gender diagnosis with deepface package in python

```
@inproceedings{qi2020wantwords,
  title={WantWords: An Open-source Online Reverse Dictionary System},
  author={Qi, Fanchao and Zhang, Lei and Yang, Yanhui and Liu, Zhiyuan and Sun, Maosong},
  booktitle={Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing: System Demonstrations},
  pages={175--181},
  year={2020}
}

@inproceedings{zhang2020multi,
  title={Multi-channel reverse dictionary model},
  author={Zhang, Lei and Qi, Fanchao and Liu, Zhiyuan and Wang, Yasheng and Liu, Qun and Sun, Maosong},
  booktitle={Proceedings of the AAAI Conference on Artificial Intelligence},
  pages={312--319},
  year={2020}
}

## code
'''
  import cv2
  from deepface import DeepFace
  
  paths = [
      'woman_1.webp',
      'man_1.webp',
      'woman_2.webp',
      'man_2.webp',
      'woman_3.webp',
      'man_3.webp',
  ]
  for path in paths:
      image = cv2.imread(path)
      analyze = DeepFace.analyze(image, actions=['gender'])
      label = cv2.putText(image,f'Gender : {analyze["gender"]}',(35,50),cv2.FONT_HERSHEY_SIMPLEX,1,(0,0,0),2)
      cv2.imshow('image',label)
      cv2.waitKey(0)
'''

  <div>
    <img src="https://github.com/arminmehraeen/Gender-Diagnosis/blob/main/images/img1.png" width="400" heght="250">
    <img src="https://github.com/arminmehraeen/Gender-Diagnosis/blob/main/images/img2.png" width="400" heght="250">
  </div>
  <div>
    <img src="https://github.com/arminmehraeen/Gender-Diagnosis/blob/main/images/img3.png" width="400" heght="250">
    <img src="https://github.com/arminmehraeen/Gender-Diagnosis/blob/main/images/img4.png" width="400" heght="250">
  </div>
  <div>
    <img src="https://github.com/arminmehraeen/Gender-Diagnosis/blob/main/images/img5.png" width="400" heght="250">
    <img src="https://github.com/arminmehraeen/Gender-Diagnosis/blob/main/images/img6.png" width="400" heght="250">
  </div>



    
    
