# Introduction
I use the model in the capsule network, change the number of convolutional layers and the size of the convolution kernel in the capsule network, and get experimental data.

# Experimental data

## Dataset-MINST
(kernel size=3*3)

![image](https://user-images.githubusercontent.com/97005274/164592668-ed1edac8-0926-44e0-91d8-e631dfef9356.png)
(kernel size=5*5)

![image](https://user-images.githubusercontent.com/97005274/164599622-90a76088-46de-4992-87c2-a6b66a279cb2.png)

(kernel size=7*7)

![image](https://user-images.githubusercontent.com/97005274/164599688-b9520a13-091c-4cb7-9c34-3bd0f91c7dab.png)

(kernel size=9*9)

![image](https://user-images.githubusercontent.com/97005274/164599763-d1fac799-1314-4d2a-b7b4-628b80e98e64.png)


## Dataset-Fasion_MINST
(kernel size=3*3)

![image](https://user-images.githubusercontent.com/97005274/164604192-20e107b3-3b75-4c03-a65c-8c81dbb85143.png)

(kernel size=5*5)

![image](https://user-images.githubusercontent.com/97005274/164605152-b5a6cc8b-5111-44e7-9808-30ac12a639f5.png)

(kernel size=7*7)

![image](https://user-images.githubusercontent.com/97005274/164605233-da242d6c-1ca3-473f-924d-046404b3e97e.png)

(kernel size=9*9)

![image](https://user-images.githubusercontent.com/97005274/164747069-66fe4a3b-d642-404e-baf2-50e41f208bed.png)


## Dataset-HMD
(kernel size=3*3)

![image](https://user-images.githubusercontent.com/97005274/164747190-737f9780-a5a0-4f1d-aa96-15d773c4ad7b.png)

(kernel size=5*5)

![image](https://user-images.githubusercontent.com/97005274/164748205-f9e2d626-1262-4856-9833-d6bc9a6407f0.png)

(kernel size=7*7)

![image](https://user-images.githubusercontent.com/97005274/164748294-7828bc3f-7d6f-461b-9bbd-a00d108100c2.png)

(kernel size=9*9)

![image](https://user-images.githubusercontent.com/97005274/164748364-4ce689a5-cfa7-418c-b501-5869e9ef25af.png)

## Dataset-Cifar10

(kernel size=3*3)

![image](https://user-images.githubusercontent.com/97005274/164749665-371f6cdd-c0c4-47d9-b687-159572b33ef4.png)

(kernel size=5*5)

![image](https://user-images.githubusercontent.com/97005274/164749801-4309f988-ab79-4da7-9a02-2e61626a8f1f.png)

(kernel size=7*7)

![image](https://user-images.githubusercontent.com/97005274/164749900-d723cc25-9db4-4681-bd93-556d8ad3688b.png)

(kernel size=9*9)

![image](https://user-images.githubusercontent.com/97005274/164749968-90837cab-a5de-4a72-a875-8ef277ca531c.png)

# Test accuracy of different convolution kernel sizes

## dataset-MINST

![image](https://user-images.githubusercontent.com/97005274/164751461-38d0a24b-0f9c-41c5-a894-6e3e280af87e.png)

## dataset-Fasion_MINST

![image](https://user-images.githubusercontent.com/97005274/164751633-56429694-d9e9-4508-98d8-9012bd33c7a0.png)

## dataset-HMD

![image](https://user-images.githubusercontent.com/97005274/164751750-108987cf-7cbb-457b-822e-27ed8bd4db09.png)

## dataset-Cifar10

![image](https://user-images.githubusercontent.com/97005274/164751804-ee8fb6c0-eb0b-4e6b-b58a-5f37bf5c8032.png)

## Compare-result
In black and white image datasets, using convolutional layers of 3 to 7 convolutional layers with a convolution size of 5×5 is better for recognition, because the receptive field of the convolution kernel size (5×5) is twice that of (3×3) , which allows more information to be captured during feature extraction when convolutional layers are stacked.

In the color image dataset, the convolution size of 3 × 3 is better for recognition when using 3 to 7 convolutional layers, because the smaller convolution kernel size can capture very subtle features. Color image comparison Complexity requires subtle features, so that the subsequent classification of the capsule network can be better
