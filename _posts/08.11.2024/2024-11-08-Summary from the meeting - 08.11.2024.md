---
title: Summary from the meeting - 08.11.2024
date: 2024-11-08
categories: 
tags: [Raspberry, job, logistics, sequencing, multiple_printers, temperature, vibration, positioning, CNNs, RNNs, ML, third]
---

Participants : Prof Engel , Prof.Menzel , Milad Herfeh
Here’s the complete summary of your recent meeting [transcribe](../transcribe): 
> *Summarized with GPT*
---

### 1. **System Architecture and Data Organization:**
   - The setup involves [OctoPrint](../OctoPrint) on a #Raspberry Pi 4, centralizing sensor data collection and job control for 3D printing. Each print job is seen as a “container” for relevant data, including [G-code](../G-code) and sensor readings, with protocols like MQTT for data exchange.
   - Consideration is given to data standards and protocols for better integration, with [CDF](../CDF) (Common Data Format) being considered for data storage due to its flexibility in handling large data sets and metadata.

### 2. **Job and Workflow Management:**
   - A print #job is defined by stages: initiation, execution, and logistics. This includes pre- and post-job logistics, such as plate preparation, cleaning, and inspection.
   - [OctoPrint](../OctoPrint) enables scheduling and triggers multiple jobs across different printers, handling #logistics and job #sequencing for streamlined workflow and preparation.
   - There’s also discussion on handling #multiple_printers, such as Printer A and Printer B, to enhance process scalability and efficiency.

### 3. **Sensor Integration and Multidimensional Data:**
   - External [Sensors](../Sensors) like acoustic sensors are considered alongside internal sensors ( #temperature, #vibration, #positioning), with data structured by sensor types (temperature, vibration, acceleration) and their measurement metadata.
   - *Complex multidimensional data handling *is anticipated, particularly for ML applications like time series prediction, classification, and control optimization.
   - Future data structuring may include embedding data into vector spaces to allow advanced data analysis and problem detection.

### 4. **Machine Learning and Large Language Models (LLMs):**
   - There’s ongoing exploration of applying [LLM](../LLM) and deep learning models (e.g., #CNNs, #RNNs) for predictive maintenance, quality monitoring, and job control across multiple printers.
   - Potential partnership with Siemens is mentioned for access to their industrial AI copilot, which could use print data for enhanced monitoring. / **Abgesagt** / 
   - The data framework being built is intended to be generic, allowing for diverse #ML approaches, including unsupervised learning (e.g., anomaly detection) and supervised learning (e.g., labeled success/failure).

### 5. **Challenges and Considerations:**
   - Ensuring data collection consistency and handling varied data types and standards is challenging, especially with non-uniform sensor capabilities across different printers.
   - OctoPrint’s compatibility with #third-party printers (e.g., Prusa, MakerBot) varies, limiting direct control over non-compliant systems.
   - The current aim is to establish a modular, reusable framework that supports scalable integration of sensors and multiple printers.

### 6. **Future Developments and Optimization:**
   - Future developments include potentially optimizing the entire workflow, not just individual printing processes, by aligning task preparation, slicing, and job sequencing across multiple printers.
   - Exploration of time-series data and high-dimensional vector representation for monitoring could lead to real-time intelligence applications, such as defect prediction and adaptive process control.

### 7. **Research and Technical Collaboration:**
   - Further discussions with experts on multidimensional data structures and vector-based data representation are planned to refine the data framework and enable advanced analysis capabilities.
   - Ongoing analysis is required to determine the best approaches for embedding data, visualizing states, and detecting concurrent defects.

---


![/assets/wiki/mermaid-diagram-2024-11-08-182230.png](assets/wiki/mermaid-diagram-2024-11-08-182230.png)




--- 
# NonAI - Content 


1. Diagram Design 
2. 