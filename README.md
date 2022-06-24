# Gender-Diagnosis
gender diagnosis with deepface package in python

# code
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
    
<br/>
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



    
    
