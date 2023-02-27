#### Meeting #1: Drone Spot Spraying at SERF with Felipe, Narmilan, Dean and Gavin on 14th February
- For undergraduate thesis work help will be given on drone flying procedure and good to get hands on experience to write for the thesis.

- In the 13 weeks, water will be sprayed. In the first flight the M300 multi-spectral camera will be flown to get the imagery. When water is present at SERF a map will be made to spray. (I will have to make the map and specify the speed, drift, spray rate, distribution rate). The T10 will be used on the second flight to spary the water. A more in-depth investigation will be needed about the functionality and limitations of the T10.

#### Meeting #2: UAV Spot Spraying pipeline with Narmilan
- micasense altum has 5 bands (rgb and red h and near infra red) altum pt??

- Fly the drone collect raw image
- for orthomosaic use agisoft metashape and pix4d 
 then raw image is .tif and each immage will have 5 band images then do orthomosaic image. Do that process for each image.

- See the image in QGIS information tools. QGIS is a good software to use for this. Open the ortho image in QGIS. 

- Do the image processing for water logging area. Collect gps coordinates of water logging location. then do spot spraying.

- use the gps for doing the do labelling of the image in QGIS. and upload to t10.
- bunding box method (OD) or segmentaiton by pixel labelling 

- overlay the images and do the labelling.

- based on requirement make region of interest and can do labelling for each roi instead of whole ortho image.

- in ML have do 5 band input and do prediction working with VI to increase input features so combination of different bands. Look at the paper reference for vegetaion indices. so now 11 input feature. 

- in my case ndvi and/or excess green and can differention plant from non vegetation. difference between water and plant. Develop using gis tool or use python script.

- raster calculator in QGIS.

- do statisitcal analysis. because now 11 input feature multi colinearity test or normality test. use for publishing papers. can stop in this step.

- training models. Classic ML methods. Can try an of XGB, RF, DL, KNN.


- Fly the t10 for spot spraying.

- Have a look white lead diesease paper. and how to do Tradiitonal ml methods and deep learning methods.



- TO DO after meeting, install QGIS and play with image -> develop VI and original image, Laballing, for pix4d. Then import the ortho into gis tool and region of interest and polygon / pixelwise labelling. 

- for image processing many avaible. for spot spraying hard to find papers.

#### Meeting #3: Understanding the necessary software with Narmilan
