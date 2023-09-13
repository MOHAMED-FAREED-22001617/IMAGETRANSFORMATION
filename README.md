# IMAGETRANSFORMATION

## Aim
To perform image transformation such as Translation, Scaling, Shearing, Reflection, Rotation and Cropping using OpenCV and Python.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import the necessary libraries and read the original image and save it as a image variable.
### Step2:
Translate the image.

### Step3:
Scale the image.

### Step4:
Shear the image.

### Step5:
Reflect of image.
### Step 6:

Rotate the image.
### Step 7:

Crop the image.
### Step 8:

Display all the Transformed images.

## Program:
```python
Developed By:MOHAMED FAREED
Register Number:
i)Image Translation
translation = np.float32([[1,0,150],[0,1,250],[0,0,1]])
translated_image = cv2.warpPerspective(original,translation,(col,row))

cv2.imshow('translated_image',translated_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

ii) Image Scaling

scaling = np.float32([[1.2,0,0],[0,1.8,0],[0,0,1]])
scaled_image = cv2.warpPerspective(original,scaling,(col,row))

cv2.imshow('scaled_image',scaled_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

iii)Image shearing


shear_x = np.float32([[1,0.7,0],[0,1,0],[0,0,1]])
shear_y = np.float32([[1,0,0],[0.3,1,0],[0,0,1]])

sheared_x= cv2.warpPerspective(original,shear_x,(col,row))
sheared_y = cv2.warpPerspective(original,shear_y,(col,row))

cv2.imshow('shear_x',sheared_x)
cv2.waitKey(0)
cv2.destroyAllWindows()

cv2.imshow('shear_y',sheared_y)
cv2.waitKey(0)
cv2.destroyAllWindows()


iv)Image Reflection

ref_x = np.float32([[1,0,0],[0,-1,row],[0,0,1]])
ref_y = np.float32([[-1,0,col],[0,1,0],[0,0,1]])

reflect_x= cv2.warpPerspective(original,ref_x,(col,row))
reflect_y = cv2.warpPerspective(original,ref_y,(col,row))

cv2.imshow('reflected_x',reflect_x)
cv2.waitKey(0)
cv2.destroyAllWindows()

cv2.imshow('reflected_y',reflect_y)
cv2.waitKey(0)
cv2.destroyAllWindows()


v)Image Rotation

angle = np.radians(15)
mat_rotate = np.float32([[np.cos(angle),-(np.sin(angle)),0],[np.sin(angle),np.cos(angle),0],[0,0,1]])
rotate_img =cv2.warpPerspective(original,mat_rotate,(col,row))

cv2.imshow('rotated',rotate_img)
cv2.waitKey(0)
cv2.destroyAllWindows()


vi)Image Cropping

cropped_img=img[10:500,25:600] 

cv2.imshow('after_cropping',cropped_img);
cv2.waitKey(0)
cv2.destroyAllWindows()



```
## Output:
### i)Image Translation
![IMG-01](https://github.com/MOHAMED-FAREED-22001617/IMAGETRANSFORMATION/assets/121412904/bdd8d609-4bdd-41f5-9ad4-b5ae0e61b494)

![IMG-02](https://github.com/MOHAMED-FAREED-22001617/IMAGETRANSFORMATION/assets/121412904/a4637d2a-2f6e-49d4-83ad-e83570ca83f6)

### ii) Image Scaling
![IMG-03](https://github.com/MOHAMED-FAREED-22001617/IMAGETRANSFORMATION/assets/121412904/745809a2-6706-4447-a74d-e5fa05eb6c19)


### iii)Image shearing
![IMG-04](https://github.com/MOHAMED-FAREED-22001617/IMAGETRANSFORMATION/assets/121412904/3e69ab1b-fa32-4363-8cc4-203268f129ee)

![IMG-05](https://github.com/MOHAMED-FAREED-22001617/IMAGETRANSFORMATION/assets/121412904/609163fd-2b23-47ac-903c-d11d930436c6)


### iv)Image Reflection
![IMG-06](https://github.com/MOHAMED-FAREED-22001617/IMAGETRANSFORMATION/assets/121412904/b3bcb1b8-fa09-4866-beab-5cc0ceeeb7b4)

![IMG-07](https://github.com/MOHAMED-FAREED-22001617/IMAGETRANSFORMATION/assets/121412904/7f213c56-aa94-43a2-817b-1a91ca87228d)

### v)Image Rotation
![IMG-08](https://github.com/MOHAMED-FAREED-22001617/IMAGETRANSFORMATION/assets/121412904/a0708946-2dc9-4e9c-9309-737e5fd35781)




### vi)Image Cropping
![IMG-09](https://github.com/MOHAMED-FAREED-22001617/IMAGETRANSFORMATION/assets/121412904/ad8cb44d-7839-4d65-a436-af167a2a7a24)
## Result: 

Thus the different image transformations such as Translation, Scaling, Shearing, Reflection, Rotation and Cropping are done using OpenCV and python programming.
