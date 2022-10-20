### Release Image generator based on GAN

#### 22.10.20. 10:00
**Update** 03_Face_Mask_Generator_based_on_GAN
- WGAN-GP GP 부분 에러 해결
- generator 와discriminator loss가 수렴되지 않으며,
 생성 이미지의 퀄리티가 좋지 않음.
**quick result**
- Loss log of generator & discriminator
<img src="https://github.com/JiwooKimm/CNUSW22_Project01_ImageClassifier/blob/master/03_ImageGenerator_GAN/figures/WGAN-GP_loss_log1_conv.png">

- Generated (fake) images

**to fix**
각 레이어를 convolution 이 아닌 fully connect 시킨다. 


#### 22.10.20.02:00
**Upload** back up file (03_Face_Mask_Generator_based_on_GAN(backup))

**Update** 03_Face_Mask_Generator_based_on_GAN 
- WGAN-GP 이용한 얼굴 이미지 생성기 작성 중 GP 부분 에러

	
