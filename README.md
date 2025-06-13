# Building-a-disaster-risk-monitoring-system-using-computer-vision
Flood detection using semantic segmentation . For the purposes of detecting flood events, I will develop a semantic segmentation model trained with labelled images that are generated from Sentinel-1 data.

### What is the purpose? 

To detect and respond to disasters (like floods) in real time using satellite data, AI models, and alerts — so authorities can act quickly and plan better.

### What is Semantic Segmentation? 

Semantic segmentation is a computer vision technique where an AI model looks at an image and labels each pixel based on the object it belongs to (e.g. water, road, vegetation).
In this case, we train a model to identify flooded areas pixel by pixel.

### Why Use Satellite Imagery?

Using satellites for flood monitoring is:

- Safer: No need to physically access dangerous flooded areas.
- Faster: No need for manual inspections.
- More reliable: Works even when the weather is bad or at night.
- We use data from the Copernicus Sentinel-1 mission, which provides C-band Synthetic Aperture Radar (SAR) data.
- SAR satellites like Sentinel-1 can see through clouds and darkness — perfect for emergency monitoring.

Key features of Sentinel-1:

- Works day and night, rain or shine.
- Delivers radar images of the Earth’s surface.
- Two satellites (1A & 1B) orbit the Earth every 6 days.
- Operates in Low Earth Orbit (LEO) for faster data updates.

More information about the Sentinel-1 mission can be found here https://directory.eoportal.org/satellite-missions/copernicus-sentinel-1 


### Deep Learning-Based Disaster Risk Monitoring System workflow 

1. Satellite remote sensors capture data (Satellites take pictures or scan the Earth from space (e.g. flood areas, land changes)
2. Data are used to (continuously) train deep learning neural network models (These images are used to train AI models that learn to recognise signs of flooding, landslides, etc). 
3. Different models and versions are managed by the model repository
4. Model inference performance is actively monitored (The system watches how well the models are doing when they run in real life — this helps catch errors early). 
5. Data are passed to the inference server (The trained models live in an inference server (here it's Triton), where they analyse new incoming data in real time). 
6. The deep learning inference results are post-processed for either (After the AI makes predictions (like detecting flood zones), those results are cleaned up and structured for use). 
7. Further analytics by 3rd party or (A third-party (like government agencies) might do extra analysis on these results). 
8. Raising alerts (If danger is detected (e.g. rising water), alerts are sent to users — on phones, computers, or public systems). 

<img width="701" alt="Screenshot 2025-06-03 at 22 20 20" src="https://github.com/user-attachments/assets/1e371666-02ff-48de-9c08-e71e7f25d2a1" />

### Why is this useful?

Helps map flood areas quickly
Supports real-time disaster response
Can predict flood direction, recommend safe routes, and help rescue teams plan
Improves resource allocation (e.g. where to send aid)


## Tools used 

* NVIDIA GPU Cloud

Register and activate a free NGC account

Generate your NGC API key and save it in a safe location


