# Building-a-disaster-risk-monitoring-system-using-computer-vision
Flood detection using semantic segmentation . For the purposes of detecting flood events, we will develop a semantic segmentation model trained with labelled images that are generated from Sentinel-1 data.



### Semantic segmentation is a computer vision technique where an AI model looks at an image and labels each pixel according to what object it belongs to.

we demonstrate the ability to create a flood detection segmentation model using satellite imagery. Using satellites to study flood is advantageous since physical access to flooded areas is limited and deploying instruments in potential flood zones can be dangerous. Furthermore, satellite remote sensing is much more efficient than manual or human-in-the-loop solutions.

To obtain detailed and valuable information for flood monitoring, satellite missions such as Copernicus Sentinel-1, provides C-band Synthetic Aperture Radar (SAR) data. Satellites that use SAR, as opposed to optical satellites that use visible or near-infrared bands, can operate day and night as well as under cloud cover. This form of radar is used to create two-dimensional images or three-dimensional reconstructions of objects, such as landscape. The two polar-orbiting Sentinel-1 satellites (Sentinel-1A and Sentinel-1B) maintain a repeat cycle of just 6 days in the Lower Earth Orbit (LEO). Satellites that orbit close to Earth in the LEO enjoy the benefits of faster orbital speed and data transfer. These features make the Sentinel-1 mission very useful for monitoring flood risk over time. Thus, a real-time AI-based remote flood level estimation via Sentinel-1 data can prove game-changing. 

More information about the Sentinel-1 mission can be found here https://directory.eoportal.org/satellite-missions/copernicus-sentinel-1 


## Deep Learning-Based Disaster Risk Monitoring System workflow 

1. Satellite remote sensors capture data
2. Data are used to (continuously) train deep learning neural network models
3. Different models and versions are managed by the model repository
4. Model inference performance is actively monitored
5. Data are passed to the inference server
6. The deep learning inference results are post-processed for either
7. Further analytics by 3rd party or
8. Raising alerts

<img width="701" alt="Screenshot 2025-06-03 at 22 20 20" src="https://github.com/user-attachments/assets/1e371666-02ff-48de-9c08-e71e7f25d2a1" />



## Tools used 

* NVIDIA GPU Cloud

Register and activate a free NGC account

Generate your NGC API key and save it in a safe location


