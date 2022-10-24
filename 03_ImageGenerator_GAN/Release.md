### Release Image generator based on GAN

#### `22.10.24 15:30`

**Update** 03_Face_Mask_Generator_based_on_GAN
- label 누락 문제 수정
- WGAN-GP model v.3
	- Optimizer: RMSprop
	- epoch: 200
	- fully-connected network

**quick results**
- loss-log 

<img src="https://github.com/JiwooKimm/CNUSW22_Project01_ImageClassifier/blob/master/03_ImageGenerator_GAN/figures/WGAN-GP_v3_loss_log1.png">

- generated images
 <img src="https:/
	/github.com/JiwooKimm/CNUSW22_Project01_ImageClassifier/blob/master/03_ImageGenerator_GAN/figures/WGAN-GP_v3_with_mask.png" width= "30">

<img src="https://github.com/JiwooKimm/CNUSW22_Project01_ImageClassifier/blob/master/03_ImageGenerator_GAN/figures/WGAN-GP_v3_without_mask.png" width= "30">


\space <span style="color: gray"> 📎 
- WGAN-GP_v3_Generator_for_Face_Mask.pt
- WGAN-GP_v3_Discriminator_for_Face_Mask.pt
- results_customWGAN-GP_v3.zip
- WGAN-GP_v3_without_mask.png
- WGAN-GP_v3_with_mask.png
- WGAN-GP_v3_loss_log2.png
- WGAN-GP_v3_loss_log1.png
</span>

#### `22.10.24 12:05`
**Update** 03_Face_Mask_Generator_based_on_GAN
#### `22.10.20 22:00`

**Update** 03_Face_Mask_Generator_based_on_GAN
- 신경망을 convolution network -> fully connected network 으로 수정

**quick result**
- loss 잘 수렴되는 것 같고, 생성 이미지의 퀄리티 나쁘지 않으나 label 생성 누락 -> with/without 마스크 구분 불가,,
- Generated (fake) images
<img src="https://github.com/JiwooKimm/CNUSW22_Project01_ImageClassifier/blob/master/03_ImageGenerator_GAN/figures/WGAN-GP_face_nolabel.png">



#### `22.10.20. 10:00`

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


#### `22.10.20.02:00`

**Upload** back up file (03_Face_Mask_Generator_based_on_GAN(backup))

**Update** 03_Face_Mask_Generator_based_on_GAN 
- WGAN-GP 이용한 얼굴 이미지 생성기 작성 중 GP 부분 에러

	
