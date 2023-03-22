## Topics to be Researched
#### Bioagent methods against malaria and dengue
- Bioagent is a bacterium, virus, protozoan, parasite, fungus, or toxin that can be used for a specfic purpose.

#### Other research or activity on drones for this purpose


#### The DJI T10 and how the GCS works 
- The DJI Agras T10 has an 8L spray tank and convinient for spraying bioagent. The battery and tank can be quickly attached and detached to make refilling more efficient.

(Specifications)
- More information on the specs can be found here: https://www.dji.com/uk/t10/specs 
- Has a Spherical Radar System

(User Manual)
https://dl.djicdn.com/downloads/t10/T10_User_Manual_v1.4_EN.pdf
- Flight modes. Default is P mode. This is positon mode. The drone will hold its position and altitude. A-mode is for Attitude, can only maintain altitude using the barometer. A mode is not used for positioning.

- Operation modes: A-B modes, Manual and Manual Plus.

- 


#### SERF & puddles of water at SERF


#### Investigate where and who sells the biofluid they talk about in the videos and papers

 
#### Papers on finding water bodies with drone and multispectral imagery


#### Vegetation indices (VI), please learn some basic ideas about VI
- What is a vegetation index? 
- Answer: A vegetation index is a mathematical formula that uses the reflectance of light from a target to determine the amount of chlorophyll in the target.  
VI or Vegetation Index is actually a spectral index, i.e. a combination of spectral band
- List of vegetation indices can be found here: https://www.indexdatabase.de/db/i.php 

- What is the difference between NDVI and EVI? Answer: NDVI is a vegetation index that uses the reflectance of near-infrared and red light to determine the amount of chlorophyll in the target. EVI is a vegetation index that uses the reflectance of near-infrared, red, and blue light to determine the amount of chlorophyll in the target.

- For the purposes of my project find Vegetation indices that can differentiate between grass and water puddles/logging. NDWI can be used, this is the Normalized Difference Water Index.

## Meetings
#### Meeting #1: Drone Spot Spraying at SERF with Felipe, Narmilan, Dean and Gavin on 14th February
- For undergraduate thesis work help will be given on drone flying procedure and good to get hands on experience to write for the thesis.

- In the 13 weeks, water will be sprayed. In the first flight the M300 multi-spectral camera will be flown to get the imagery. When water is present at SERF a map will be made to spray. (I will have to make the map and specify the speed, drift, spray rate, distribution rate). The T10 will be used on the second flight to spary the water. A more in-depth investigation will be needed about the functionality and limitations of the T10.

#### Meeting #2: UAV Spot Spraying pipeline with Narmilan 21st February
- micasense altum pt has 5 bands (rgb and red edge and near infra red). (More info on the altum can be found here: https://www.integraldrones.com.au/product/micasense-altum-pt/)

- Fly the drone collect raw image
- For orthomosaic use agisoft metashape and pix4d 
 the raw image will be in .tif format and each immage will have 5 band images. Use this to do the orthomosaic image. Do that process for each image.

- See the image in QGIS information tools. QGIS is a good software to use for this. Open the ortho image in QGIS. 

- Do the image processing for water logging area. Collect gps coordinates of water logging location. then do spot spraying.

- Use the gps for doing the do labelling of the image in QGIS. and upload to t10.
- Bounding box method (Object Detection) or Segmentation method by pixel labelling 
- Overlay the images and do the labelling.

- Based on requirement make region of interest and can do labelling for each roi instead of whole ortho image.

- In ML have to do 5 band input and do prediction working with VI to increase input features so combination of different bands. Look at the paper reference for vegetaion indices. so now 11 input feature (5 input bands and the 6 vegetation indices). 

- In my case ndvi and/or excess green and can differention plant from non vegetation. difference between water and plant. Develop using gis tool or use python script.

- raster calculator in QGIS.

- do statisitcal analysis. because now 11 input feature multi colinearity test or normality test. use for publishing papers. can stop in this step.

- training models. Classic ML methods. Can try an of XGB, RF, DL, KNN.


- Fly the t10 for spot spraying.

- Have a look white lead diesease paper. and how to do Tradiitonal ml methods and deep learning methods.



- TO DO after meeting, install QGIS and play with image -> develop VI and original image, Laballing, for pix4d. Then import the ortho into gis tool and region of interest and polygon / pixelwise labelling. 

- for image processing many avaible. for spot spraying hard to find papers.

#### Meeting #3: Understanding the necessary software with Narmilan 28th February

Software used: Agisoft Metasoft to create the ortho then import into QGIS for Cropping/ROI, Labelling and ML Processing

Agisoft Metashape:
Creating and Exporting the ortho can be found here for the P4:
https://agisoft.freshdesk.com/support/solutions/articles/31000159853-dji-phantom-4-multispectral-data-processing

For my project where the multispectral camera is used the following tutorial can be used
https://agisoft.freshdesk.com/support/solutions/articles/31000148381-micasense-altum-processing-workflow-including-reflectance-calibration-in-agisoft-metashape-professi

Add the images and align. Use moderate or low quality.
Export the image to QGIS.


QGIS:
Creating Shape file layer
Save as roi
Use as a polygon
Create it
Id initally set to 0

Raster Calculator based on the vegetation index

Labelling with id and class. 


Remeber which bands correspond

#### Meeting #4: Meeting with Felipe 9th March
- Things to clarify with felipe
a) Project deliverables
b) Next steps with flying the drone m300
c) licensing and other things needed for me
d) For assessment. Requirements 

-> Moved these meeting notes with felipe to Work Progress reports

#### Meeting #5: Narmilan 14th March 
- The JPG image is the rgb -> single camera
- The tiff image is mutli-spectral -> when seecting this use multi camera -> sort to tiff file 
- TO DO process pipeline for developing the orthomosaic (ariel and ground data)
- TO DO develop vi with orthomosaic image
- TO DO HSE Hub email refer to do the risk assessment with color (once done check with felipe)
- Same email has info and purpose and useful tips
- QUT Wiki ariel operations
- Make the gaant chart into a weekly chart (check with lecturer)
- this is multi so bring ortho and VI for ndvi ndre and exg 
- batch processing and correct order (align photos mesh an otho)
- There may be error when doing exporting images so there might be the need to do some raser transform or normalisation with the color bands. 
- gcp correection or use rtk  for high accuracy n ortho image as to where it is. 
- camera calibration using reflecting panel 
- Band 1 -> B  
- Band 2 -> G
- Band 3 -> R
- Band 4 -> Red Edge
- Band 5 -> Near infra red 

- When exporting the othomosaic the band 6 might appear which is the alpha channel that can be unchecked.

- Once in QGIS do rastor calculation
- NDVI = (Band 5 - Band 3) /(Band 3 + Band 5) where (NIR-R)/(NIR + R)
- NDRE = (Band 5 - Band 4 ) / (Band 5 + Band 4 ) where ( NIR - red edge ) / ( NIR + red edge )
- EXG = 2 * Green - Red - Blue

- TO DO Re check all the images and re upload to seperate files
- TO DO organize the folder for processing and better names


#### Meeting #6:
after VI
roi => to make the roi you need to make a vector 
polygon


Clip the ROI => 
iterate over later when clipping raster by mask layer

use power point

![thumbnail_image (1)](https://user-images.githubusercontent.com/71302996/227064213-607c293e-67c8-4f6a-85ff-ac90282b8d9b.png)
![thumbnail_image (2)](https://user-images.githubusercontent.com/71302996/227064227-c250b701-5faf-43b8-8e13-b24a9fa813d0.png)



#### Meeting #7:

#### Meeting #8:

#### Meeting #9:

#### Meeting #10:

#### Meeting #11:

#### Meeting #12:

#### Meeting #13:

#### Meeting #14:

#### Meeting #15:

#### Meeting #16:

#### Meeting #17:

#### Meeting #18:

#### Meeting #19:

#### Meeting #20:


## Lectures, Resources, Slides
#### Week 1
- Learning outcomes: Follow the style guide. 
![image](https://user-images.githubusercontent.com/71302996/223206192-e2edfff7-0274-429f-a37c-da38ff6ee481.png)
![image](https://user-images.githubusercontent.com/71302996/223206231-fbcc67db-36b3-44e0-9119-455cd027f43e.png)

#### Week 2
- Learning outcomes:

- TO DO by the end of the week:

- Risk Assessment. Fill out the risk assessment form. General HSE. When doing risk assessment evaluate all options taht pose a risk -> the story about how the oil rig or such catching fire bt people got injured due to jump off the rig. 

#### Week 3
- Things to check at lecture => 
1) Format of the work perfomance logs are correct (Agenda and discussion is fiulled out before the meeting and the rest is done during. The report will then be mailed to felipe within 24hrs of the meeting)
2) Deliverables for week 4 and if there are latex templates and can we get full marks with current template
3) About completing the HSE
