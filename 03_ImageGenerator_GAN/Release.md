### Release Image generator based on GAN
#### 22.10.20 22:00
**Update** 03_Face_Mask_Generator_based_on_GAN
- 신경망을 fully connection 으로 수정

**quick result**
- loss 잘 수렴되는 것 같고, 생성 이미지의 퀄리티 나쁘지 않으나 label 생성 누락 -> with/without 마스크 구분 불가,,
<img src-"https://github.com/JiwooKimm/CNUSW22_Project01_ImageClassifier/blob/master/03_ImageGenerator_GAN/figures/WGAN-GP_face_nolabel.png">



#### 22.10.20. 10:00
**Update** 03_Face_Mask_Generator_based_on_GAN
- WGAN-GP GP 부분 에러 해결
 
**quick result**
- generator 와discriminator loss가 수렴되지 않으며,
 생성 이미지의 퀄리티가 좋지 않음.
- Loss log of generator & discriminator
<img src="https://github.com/JiwooKimm/CNUSW22_Project01_ImageClassifier/blob/master/03_ImageGenerator_GAN/figures/WGAN-GP_loss_log1_conv.png">

- Generated (fake) images
<img src= "https://github.com/JiwooKimm/CNUSW22_Project01_ImageClassifier/blob/master/03_ImageGenerator_GAN/figures/WGAN-GP_face_maskoff_-_conv.png">

<img src= "https://github.com/JiwooKimm/CNUSW22_Project01_ImageClassifier/blob/master/03_ImageGenerator_GAN/figures/WGAN-GP_face_maskon_-_conv.png">
																		   
**to fix**
각 레이어를 convolution 이 아닌 fully connect 시킨다. 


#### 22.10.20.02:00
**Upload** back up file (03_Face_Mask_Generator_based_on_GAN(backup))

**Update** 03_Face_Mask_Generator_based_on_GAN 
- WGAN-GP 이용한 얼굴 이미지 생성기 작성 중 GP 부분 에러

	
