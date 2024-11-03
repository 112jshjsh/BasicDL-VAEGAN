# BasicDL-VAEGAN
<b> 2023-2 Basic Deep Learning </b> <br/>
Pytorch를 활용한 GAN과 VAE 구현
### Dataset
Flowers imitation (https://www.kaggle.com/datasets/safiullina/flowers-imitation/code)

---

## GAN
CNN 구조와 GAN을 결합한 DCGAN 모델

|Generator|Discriminator|Settings|
|------|---|---|
|ConvTranspose2d|Conv2d|Optimizer: Adam|
|BatchNorm2d|BatchNorm2d|Batch size: 128|
|ReLU|LeakyReLU|Learning Rate: 1e-4|
|Tanh|Sigmoid|Epoch: 30, 100, 200|

### Result
![Result_GAN](https://github.com/user-attachments/assets/dc5a5ee9-f0f2-40b5-8447-5cea9c38cd6e)

---

## VAE

|Encoder|Decoder|Settings|
|------|---|---|
|Conv2d|ConvTranspose2d|Optimizer: Adam|
|ReLU|ReLU|Batch size: 32|
| |Sigmoid|Learning Rate: 1e-3|
| | |Epoch: 30, 100, 200|

### Result
![Result_VAE](https://github.com/user-attachments/assets/74063bb5-1c15-4b28-a77a-ebb3235150c5)
