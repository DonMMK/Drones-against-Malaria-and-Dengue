# Literature Review: Drones against Malaria and Dengue

#### Agricultural Drone Industry Insight Report
Link: https://ag.dji.com/newsroom/ag-news-en-ag2022



#### UAV-spray application in vineyards and spray system adjustments effects on canopy deposit, coverage, and off-target losses
[UAV-spray application in vineywards](https://github.com/DonMMK/Drones-against-Malaria-and-Dengue/blob/main/Literature%20Review/1-s2.0-S004896972204390X-main.pdf)  

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

-  Results for each variable changed 
1. Band spray affects application efficiency by increasing canopy deposition.
2. Conventional nozzle type showed better coverage and lower ground loss.
3. 
4. The conventional airblast sprayer, operated at a low spray application rate, showed higher canopy coverage and lower
ground losses in comparison to the best UAV-spray system configuration.

(Introduction)  
- In mechanized commercial vinyards pesticide residue in food reports are increasing (0.4% to 0.9%) (EFSA, 2021).
- During spray applications a considerable amount of chemical becomes off-target losses.
- Precision agricultural techniques have improved the spary applications resulkting in benefits in reducing environmental and human contamination risks, improving PPP benefits and raising food quality standards.
- Aerial Spraying from UAVs is challenegin in terms of UAV path planning definition but in recent years has been spreading worldwide. It is largely used in Asia.
- 1) Cruise speed 2) flight height 3) number of spray passages per each row 4) nozzle size and type 5) liquid pressure 6) number of active nozzles.
- The downwash effect of UAV rotors is important in increasing the canopy deposition in crops, especially in bush or tree crops. This effect is used to move foliage and convey droplets into the canopy, increasing the chances of reaching the innermost leaves. Researchers have highlighted difficulties in penetrating canopies due to their shape and density in citrus orchards. The UAV path and flight mode are crucial in relation to the planting system and tree shapes.

(Materials and Methods) 
2.1 UAV-spary system
- Used a DJI Matrice 600 Pro. Other specifics used are mentioned but not important for the purposes of my investigation as using a M300 and T10 drone.

2.2 Experimental Design   
- Explore the 12 different configurations used for the various tests. Configurations attached below.
![image](https://user-images.githubusercontent.com/71302996/222997744-864680e0-36fa-4b5e-a9ed-1b21d6339a68.png)

2.3 Experimental Layout  
- nothing to add to my experiment
 
2.4 Field test and vineyard characteristics  
- nothing to add to my experiment

2.5 Enviromental conditions monitoring  
-

2.6 Droplet size spectra characteristics

2.7 Spray mixture and tracer concentration

2.7.1 Spray deposit quantiﬁcation

2.8. Images analysis for spray coverage characterisation

2.9. Statistical and data analysis

(Results and discussion)
3.1. Canopy deposit

3.2. Canopy coverage

3.3. Ground deposit

3.4. In-depth analysis of the 1-way band ﬂight mode

3.4.1. Canopy deposit: spatial canopy spray deposit distribution and canopy penetration

3.4.2. Ground deposit: spatial distribution of the ground losses

3.5. Comparison between UAV and airblast sprayers

(Conclusion)  
- The field trials allowed to identify which of the operational parameters were optimal for vineyard spraying.
- 1) Flight mode was the paramter that affected spraying the most. UAV is aligned with the vine row orientation, made it possible to target the spray on the crop canopy as much as possible, thus maximising the deposition and minimising the off target losses on the ground.
- 2) Nozzle type also affects the efficiency of the application
- 3) Cruise speed was set to 3ms-1 to reduce spray loses
- 4) The spray rate which was set for 53 L ha-1 was demonstrated to be insufficient to guarantee an adequate spray deposit density for insecticide or fungicide spray applications.
- 5) The spray application rate must be increased using the UAV-spray system
- 6) Deposit distribution shows how the relative distance between the spray source and the target is a key parameter irrespective of application technique.

#### Key Takeaways


#### Detection of White Leaf Disease in Sugarcane Crops Using UAV-Derived RGB Imagery with Existing Deep Learning Models
[Leak detection in Water Transmission Systems](https://github.com/DonMMK/Drones-against-Malaria-and-Dengue/blob/main/Literature%20Review/remotesensing-14-06137.pdf)  

##### Important points
(Abstract)
- Remote sensing techniques based on UAVs and DL can be used to detect objects of interest - in this instance it will be detecting white leaf disease which is an economically significant disease in the sugarcane industry.
- Uses 3 RGB bands for detections. 
- Used exisiting mdoels sucha s the YOLOv5, YOLOR,DETR and faster R-CNN models for detection - the yolov5 was the best and detr was the worst. 

(Introduction) 
- For the purposes of detection of agricultural dieseases the use of small unmanned aerial vehicels along with the use of AI detection techniques was established to be the most effective method.
- Comparison of traditional AI methods and emerging DL techniques 
- About the efficiency of yolo models and ability to draw bounding boxes
- 

(Methodology)  
2.1. Process Pipeline
- acquisition, pre-processing, labelling, DL architecture, and prediction
![image](https://user-images.githubusercontent.com/71302996/223220972-9343c2bd-b829-4b97-82ad-0397d55cdcd6.png)

2.2. Study Area
- sri lanka

2.3. UAV Image Acquisition
- DJI Phantom 4 was used with a real-time kinematic module. 

2.4. Ground Truth Data Collection
- Ground truth tags were added adjacent to the plants with WLD.

2.5. Image Orthomosaics
- Initial image pre-processing consisted of using Agisoft Metashape to create RGB Orthomosaics. 
- This consisted of mainly alignment, 2.5D digital elevation model (DEM) generation, and orthomosaic creation. 

2.6. Image Tiles
- na

2.7. Image Augmentation
- To increase the model's performance, augementation was used on the training and validation set images. (Augementation only doen on validation data set under certain circumstances).

2.8 Image Labelling
- Use LabelImg to label the images. (Python based image labelling tool)

2.9. Steps in Different DL Models
- ?

2.9.1. YOLOv5
- Used google colab to train a cloned instance of yolo v5.

2.9.2. YOLOR
- similar to the yolo v5 but has pre-trained weights.

2.9.3 DETR
- converted from yolo to coco (.txt to .json) 
- process similar to yolo R

2.9.4 Faster R-CNN
- used detectron2 library to train the model.

2.10 Evaluation Metrics
- 1) Precision = mean of total number of correctly detected WLD images / total number of detected WLD images.
- 2) Recall = average of total number of correctly detected WLD images / total number of successfully identified and undetected images.
- 3) Intersection over union (IoU) = mean of the intersection of the ground truth and predicted bounding boxes / mean of the union of the ground truth and predicted bounding boxes.
- 4) mAP = mean of the average precision (AP) of all classes. Q is the number of classes.  

(Results)  
3.1 Visual Analysis of Evaluation Indicators during Training 
- Wandb was used to track the training process of the DL models.

3.2 Comparison of DL model performances
![image](https://user-images.githubusercontent.com/71302996/223305584-8e26c88d-3f1b-490d-a9f6-fb96347d1bf2.png)

- overral the yolo v5 model was the best performing model.

3.3 Training Duration 
- YOLOv5 (6h) , YOLOR (12h), DETR (30h), Faster R-CNN (3h) 
3.4 Bounding Box Detection Results from the Different DL Models

3.5 Model Comparison with previous work

(Discussion)

(Conclusion)  

#### Key Takeaways


#### Unmanned aerial vehicles for surveillance and control of vectors of malaria and other vector‑borne diseases
[Leak detection in Water Transmission Systems](https://github.com/DonMMK/Drones-against-Malaria-and-Dengue/blob/main/Literature%20Review/s12936-022-04414-0.pdf)  

##### Important points
(Highlights)  


(Abstract)
- Vector borne dieseases cause severe public health and economic impacts to over half the global population
- Typical methods of treating this larvae is laborious and slow. UAV use has rapidly expanded and has growing literature describing their potential applications.
- UAVs are highly mobile are able to reach remote areas that might be inaccessible to other ground teams.
- UAV's capabilities and limitations need to be assessed.
- Surveillance, Deployment of payloads in comparison to current conventional methods   

(Background)
- "Vector-borne diseases (VBDs) are a leading cause of global morbidity and mortality, claiming over 700,000 lives annually with over half of the world’s population at risk of infection by at least one of these diseases" [WHO. Vector-borne diseases. Geneva: World Health Organization; 2017.] 
- "insecticide resistance in
vectors and changes in land use that may bring human
populations into greater contact with vector"
- "The key capabilities of UAVs are mobility and vantage point; aerial vehicles can rapidly transport sensors or a deployable payload (the cargo or equipment being carried by the UAV) over difficult terrain as well as obtain a bird’s eye view of an area of interest" [Kim J, Kim S, Ju C, Son HI. Unmanned aerial vehicles in agriculture. A
review of perspective of platform, control, and applications. IEEE Access.
2019;7:105100–15.]
- "Emerging inexpensive commercial UAV's allows vector control programmes to acheive these objectives at an unprecedented speed and scale"
- Two methods of combating VBD is to use UAV's as a surveillance tool (sensors, ir, multi spec camera). Secondly UAV's used to deliver vector control interventions to target site.

(Searching the literature)
- Used PubMed database

(UAV use in vector habitat surveillance)
- "The abundance and distribution of malaria transmitting mosquitoes is dependent on the availability of water bodies to act as breeding sites"
- To effectivley target the larvae up to date information needs to be collected about the locations. This can be done via UAVs with sensory equipment. 
- Important to note that the water that may be muddy or covered by vegetation may be missed by visible spectrum sesnors. Hyperspectral sensors can detect water bodies by thier thermal signature
- These drones can be used for rooftops that would otherwise be inaccessible by the technicians but this requires the local communites/law to be assessed prior to the flight
- Paper showing this works well in Australia Sarira TV, Clarke K, Weinstein P, Koh LP, Lewis M. Rapid identification of
shallow inundation for mosquito disease mitigation using drone-derived
multispectral imagery. Geospat Health. 2020;15:1.
- UAV limitations => susceptibility to windspeed and precipitation, limited battery life and resulting flight range as well as their dependance on manual control by a human operator.
- vector control needs to be utillized when there is higher levels of rain which has negative implications on the ability to fly lightweight UAVs effectively.

(Considerations in selecting the appropriate UAV)
- Multi-rotor systems and the other being Fixed wing uavs

(Regulations on the use of UAVs for malaria control)
- "Regulations may also add hidden costs to UAV opera- tions as certain countries may require license fees or costly local operator courses [34]. Perceptions of UAV use by the public may also vary from place to place [90, 91], though key concerns tended to focus on physi- cal safety and privacy. Consequently, it is advisable to conduct community engagement work prior to com- mencing operations as well as to include information on drones in broader educational materials on disease control"

- UAVs good for terrain where it is inaccessible by conventional ground based methods.
- These UAVs are also good because they can deploy payloads which make them suitable for the release of control agents at target locations that might otherwise be inaccessible.
- "In particular, the growing market for UAVs that can transport and deploy large payloads of pesticides across extended flights for agricultural purposes may address the aforementioned issues of short range and payload capacity of UAVs currently used for insecticide spraying in malaria control. " <= addresses why we look at agriculture.
- Accessing the scalability of UAV use for vector and surveillance and control there needs to be a fuel and electricity efficiency.



#### UAV-based multispectral vegetation indices for assessing the interactive effects of water and nitrogen in iriigated horticultural crops production under tropical sub-humid conditions
[UAV-based multispectral vegetation indices](https://github.com/DonMMK/Drones-against-Malaria-and-Dengue/blob/main/Literature%20Review/1-s2.0-S0378377422000634-main.pdf)  

##### Important points
(Highlights)  


(Abstract)


(Introduction) 


(Materials and Methods)  


(Result and Discussion)  


(Conclusion)  


#### Key Takeaways


#### High accuracy detection of malaria vector larval habits using drone-based multispectral imagery
[High accuracy detection of malaria vector larval habits](https://github.com/DonMMK/Drones-against-Malaria-and-Dengue/blob/main/Literature%20Review/High-accuracy%20detection%20of%20malaria%20vector.pdf)  

##### Important points
(Abstract)
- Interest in larval source management (LSM) as an adjunct intervention to control and elimi- nate malaria transmission has recently increased mainly because long-lasting insecticidal nets (LLINs) and indoor residual spray (IRS) are ineffective against exophagic and exophilic mosquitoes
- This study was able to distinguish between water bodies using high resolution multispectral imagery. 

(Introduction) 
- "The decline in their efficiency is associ- ated mainly with: a) insecticide contact avoidance by early-exiting behavior of mosquitoes feeding indoors [3]; b) increased outdoor feeding and transmission; c) zoophilic behavior; and d) insecticide resistance"
- Due to vegetation it can be hard to detect ground truths
- "Transmission occurs mainly during the rainy season, January—June, linked to river levels and mosquito abundance"
- " Our main objective was to provide proof-of-concept of the suitability of high-resolution imagery (RGB band) to map Ny. darlingi aquatic habitats. Multi-spectral imaging data (including the normalized difference vegetation index- NDVI) was used to achieve sufficient resolution to identify water bodies potentially colonized by Ny. darlingi."

(Methods: Ethics Approval)

(Methods: Study Areas)
- Mazan district (Maynas Province, Loreto Department, Peru
- 

(Methods: Study Design)
- 4 places inspected at three times in the year:in September and November 2016 (dry season) and March 2017 (rainy season)

(Methods: Data Collection)

(Methods: Drone surveys)
- DJI Phantom 4 Pro w/ RGB and DJI GO 4 app
- 3DR Solo (3D Robotics, California, US)  w/ Sequoia Sensor (G R RE NIR) and 3DR solo app
- Pix4D and ipad
- 

(Laboratory Procedures)
- DNA gene analysed

(Data Processing - Orthomosaic Construction)
- Agisoft Photoscan Pro to create and orthomosaic images
- GCP needed if position of drone not captured using on board GPS
- Process of ortho : (1) photo alignment (accuracy: highest; generic preselec- tion active, reference preselection active; Key point limit: 80,000; adaptive camera model fitting active); (2) dense cloud building (quality: high; depth filtering: aggressive); (3) digital elevation model (DEM) building (geographic projection using WGS 84 (EPSG:4326); resolution of 0.1 m and 0.02 m per pixel for the RGB and multispectral images respectively; interpolation: extrapolated; all point classes to generate digital surface model); (4) orthomosaic building (input surface: DEM; blending mode: mosaic; resolution of 0.1 m and 0.02 m per pixel for the RGB and multispectral images respectively).

- NDVI = (NIR) - (R) / (NIR + R)

(Image Classification)
- Using Google Earth Engine
- RF classification use pre-labeled data as input

(Results - Mosquito breeding sites)
- From all water bodies inspected, 18 (58%) were considered negative and 13 (42%) consistently positive for the presence of Ny. darlingi immature stag

(Orthomosaics)
- 

(Discussion)
- "drone-based high-resolution mapping of Ny. darlingi breeding sites in the Amazon region. Both RBG and multispectral imagery were successfully acquired, allowing the analysis of a greater number of water bodies than ground field inspection, as well as the determination of local characteristics of Ny. darlingi habitats. Overall, the most important result of this study is the accurate classification of water bodies that enables discrimination between those that are consistently colonized by Ny. darlingi immature stages and those that are not. We believe that this strategy represents a new tool for tailored interventions for control and surveillance of malaria transmission in rural communi- ties of the Peruvian Amazon and elsewhere"

(Conclusions)
- In summary, the use of high-resolution imagery can provide a better understanding of environment-related disease changes and can play a meaningful part in the development of decision-support tools. Our findings back the use of a low-cost UAVs and a freely available planetary cloud-based platform to achieve a highly accurate classification of the differential spectral signature of water bodies that harbor Ny. darlingi larvae and those that do not, in the Amazon region. This strategy might be generalizable to similar contexts elsewhere, resulting in new ways to control and survey malaria in affected settings, in combination with existing approaches.

#### Leak detection in Water Transmission Systems by multispectral Remote Sensing with Airplane and UAV
[Leak detection in Water Transmission Systems](https://github.com/DonMMK/Drones-against-Malaria-and-Dengue/blob/main/Literature%20Review/IGARSS2019.pdf)  

##### Important points
(Highlights)  


(Abstract)


(Introduction) 


(Materials and Methods)  


(Result and Discussion)  


(Conclusion)  

#### Key Takeaways
