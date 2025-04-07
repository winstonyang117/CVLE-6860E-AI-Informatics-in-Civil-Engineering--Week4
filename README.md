# CVLE 6860E AI & Informatics in Civil Engineering 

<p align="center">
    <img src="contents/UGA.PNG" width="500"/>
</p>

<p align="center">
    🏛️ <a href="https://smil.engr.uga.edu/"><b>Smart Mobility and Infrastructure Lab</b></a>
</p>

## Week 4: Nighttime Vechicle Detection and Classification
The disproportionate risk of roadway fatalities on rural roads, where 43% of all roadway fatalities occur despite only 19% of the US population living in these areas, underscores a critical and worsening challenge in transportation safety. This is largely due to unique challenges associated with rural roads (e.g., varying roadway geometrics, frequent animal crossings, reduced cell phone and communication coverage). 
<p align="center">
    <img src="contents/rural_stats.png" width="700"/>
</p>
Nighttime vehicle detection is crucial for various transportation safety and automation systems. At night, reduced visibility due to low lighting conditions significantly increases the risk of traffic accidents. Detecting vehicles accurately during nighttime plays a key role in improving road safety, managing traffic, and enhancing the effectiveness of intelligent transportation systems (ITS).
Rural roads often lack the infrastructure and safety features found in cities, leading to higher accident rates, particularly at night.
Deploying deep learning models for nighttime vehicle detection offers significant advantages compared to traditional methods. Deep learning, particularly using convolutional neural networks (CNNs) and other advanced architectures, can effectively handle the challenges of low-light conditions, environmental variability, and complex data interpretation. 


### Current bottlenecks and challenges:
* **Low Illumination and Contrast**: Nighttime environments suffer from poor lighting conditions, making it difficult for deep learning models to distinguish between vehicles and the background. Low illumination also reduces the overall image contrast, making it challenging for models to detect vehicle boundaries accurately.
* **Headlight and Reflection Glare**: The presence of strong headlight glare and reflections from vehicles can confuse the models, as these bright spots can either be misinterpreted as vehicles or obscure the actual objects of interest.
* **Noise and Low-Quality Images**: Nighttime images often suffer from noise, motion blur, and low resolution due to reduced sensor performance in low light. This degrades the quality of data used for detection and can negatively impact the model's accuracy.
* **Limited Training Data**: There is a scarcity of large, diverse, and annotated nighttime vehicle datasets. Models trained predominantly on daytime data do not generalize well to nighttime scenarios, leading to poor detection performance.
* **Domain Adaptation Issues**: Deep learning models that are trained on daytime images often perform poorly at night, as the features and environmental conditions differ significantly. Adapting models to function well across both daytime and nighttime scenarios is a major challenge.

<p align="center">
  <img src="contents/night_sample.gif" width="600"/><br/>
<em>Nighttime Video from the Roadside Traffic Camera in California Highway</em>
</p>

<p align="center">
  <img src="contents/night_sample_2_v2.gif" width="600"/><br/>
<em>Nighttime Video from the Roadside Traffic Camera in South Carolina Highway</em>
</p>


### AI Empowered Augmentation Methods - Generative Adversarial Network (GAN):
The **generator** learns to generate plausible data. The generated instances become negative training examples for the discriminator.
The **discriminator** learns to distinguish the generator's fake data from real data. The discriminator penalizes the generator for producing implausible results 
















<p align="center">
  <img src="contents/ca_sample_yolo12.gif" width="600"/><br/>
<em>Daytime Detection and Classification via Raw YOLO12 Model</em>
</p>

<p align="center">
  <img src="contents/sc_sample_yolo12_night.gif" width="600"/><br/>
<em>Nighttime Detection and Classification via Raw YOLO12 Model</em>
</p>


