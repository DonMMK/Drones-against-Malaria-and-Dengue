# Thesis Proposal: Drones against Malaria and Dengue


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
- What is a vegetation index? Answer: A vegetation index is a mathematical formula that uses the reflectance of light from a target to determine the amount of chlorophyll in the target.
- What are Vegetation indices? (Taken from Narmilan's Paper: detection of White Leaf Disease...) 

- What is the difference between NDVI and EVI? Answer: NDVI is a vegetation index that uses the reflectance of near-infrared and red light to determine the amount of chlorophyll in the target. EVI is a vegetation index that uses the reflectance of near-infrared, red, and blue light to determine the amount of chlorophyll in the target.

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

## Literature Review & Published Papers
#### Agricultural Drone Industry Insight Report
Link: https://ag.dji.com/newsroom/ag-news-en-ag2022



#### UAV-spray application in vineyards and spray system adjustments effects on canopy deposit, coverage, and off-target losses
[UAV-spray application in vineywards](https://github.com/DonMMK/Drones-against-Malaria-and-Dengue/blob/main/Read/1-s2.0-S004896972204390X-main.pdf)  

##### Important points
(Highlights)  

- The UAV-spray system flight path plays a
key role in vineyards spray applications.
- Conventional nozzle combined with high UAV speed results in higher canopy deposit: 
  * What is canopy deposit?
- Spray applications above the canopy maximised deposition compared to broadcast ones.
- Spray applications above the canopy also minimised ground losses.
- Spray volume rate from UAV must be increased to guarantee a minimum deposit density.

(Abstract)  
- When the spray process is improved less bioagent is used which reduces contamination of the environment and the cost of the bioagent. Maximise the amount of bioagent that is deposited on the target and reduce off-target losses.
- Variables changed across 12 configurations
1. Different flight modes(band, broadcast)
2. Different nozzle types (conventional and air inclusion) 
3. Different UAV cruise speeds (1 and 3 ms-1)
4. Using UAV spray system or airblast spray system

-  Results for each varibale changed 
1. Band spray affects application efficiency by increasing canopy deposition.
2. Conventional nozzle type showed better coverage and lower ground loss.
3. 
4. The conventional airblast sprayer, operated at a low spray application rate, showed higher canopy coverage and lower
ground losses in comparison to the best UAV-spray system configuration.

(Introduction)  
- In mechanized commercial vinyards pesticide residue in food reports are increasing (0.4% to 0.9%).
- 

(Materials and Methods)  


(Result and Discussion)  


(Conclusion)  




#### Key Takeaways


#### UAV-based multispectral vegetation indices for assessing the interactive effects of water and nitrogen in iriigated horticultural crops production under tropical sub-humid conditions
[UAV-based multispectral vegetation indices](https://github.com/DonMMK/Drones-against-Malaria-and-Dengue/blob/main/Read/1-s2.0-S0378377422000634-main.pdf)  

##### Important points
(Highlights)  


(Abstract)


(Introduction) 


(Materials and Methods)  


(Result and Discussion)  


(Conclusion)  


#### Key Takeaways


#### High accuracy detection of malaria vector larval habits using drone-based multispectral imagery
[High accuracy detection of malaria vector larval habits](https://github.com/DonMMK/Drones-against-Malaria-and-Dengue/blob/main/Read/High-accuracy%20detection%20of%20malaria%20vector.pdf)  

##### Important points
(Highlights)  


(Abstract)


(Introduction) 


(Materials and Methods)  


(Result and Discussion)  


(Conclusion)  

#### Key Takeaways


#### Leak detection in Water Transmission Systems by multispectral Remote Sensing with Airplane and UAV
[Leak detection in Water Transmission Systems](https://github.com/DonMMK/Drones-against-Malaria-and-Dengue/blob/main/Read/IGARSS2019.pdf)  

##### Important points
(Highlights)  


(Abstract)


(Introduction) 


(Materials and Methods)  


(Result and Discussion)  


(Conclusion)  

#### Key Takeaways

