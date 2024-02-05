At this report I’m going to write about automating an image in the blog. My problem was in the area of images in the markdown file. I'm gonna use some HTML and CSS.

### 1:

Probably the common way to add an image in the blog is to refer to issues section and upload the image there and use the link to display the image in the blog. For example:
```
![SS-KH_security-camera-pros-and-cons-HRO](https://github.com/23W-GBAC/SinaNajafi1/assets/148863702/c9f4c82b-66fe-410f-80c6-32244d8a2bb7)
```
I used to upload my images with these links. I realized that I need to add some features to my images.

### 2:

When we add an image like this we can’t adjust the location of the image. For example if we want to put the image in the center of the page with a description, we should use HTML code within the Markdown file:
```
•	<div style="text-align:center;">
  <img src="your_image_url_here" alt="Your Image Alt Text">
</div>
•	<p align="center">
  <img src="url_here" alt="Alt Text" style="margin-top: 20px;">
</p>
```
But these two codes are not useable probably because of github limitations. Also they leave our images as a descripted link. As a final solution to align the image I used the following code in part 3.

### 3:
If we want to see the actual image directly, we can simply use the following code and align it to center:
```
<p align="center">
  <img src=”url_of_image” >
</p>
```
### 4:
Furthermore, I wanted to adjust my images size. I used to use photoshop before, but this is not efficient here in my blog because of two reasons, Cost and resource.

Codes for changing size of image:
```
•	![Alt](url) | width=X
```
```
•	![Alt](url) =X*Y
```
Most likely these two will not work, so final solution is:
```
<img src=”url_of_image” width=”x” height=”y” />
```
