# 🎯Unit A Case Study + Final Term Project, W16
## Practice Lab

### Step 1 Input Your Prompt and Information and Enable “Canvas”
<img width="706" height="620" alt="image" src="https://github.com/user-attachments/assets/d9a6e875-c22a-4416-869c-2bc6b1163ebc" />

### Step 2 Review and Automatic Coding by Google Gemini
<img width="1913" height="999" alt="image" src="https://github.com/user-attachments/assets/aa83cd47-a8d4-4401-ac98-99398cc6e070" />

### Step 3 Review & Play Your Result; finally, add your key take aways
<img width="1904" height="799" alt="image" src="https://github.com/user-attachments/assets/3e14540e-a3f4-4874-a435-84adfdbdc35a" />

## Missions & GitHub 
### 1. Create a new NotebookLM then load the YouTube Video, the paper, and Fast Research (e.g., “What's is the latest status of food bank in US?”) 
<img width="716" height="452" alt="image" src="https://github.com/user-attachments/assets/4f5c5917-1372-4ea6-8f58-390ed1353734" />

### Q1: Please introduce the case use from social pain points, solutions, and information asystems which they can use?

FvDesigner provides a comprehensive HMI (Human Machine Interface) solution to address modern industrial challenges:

**Social and Industrial Pain Points**

• Remote Maintenance Challenges: Difficulty managing and troubleshooting equipment in distant locations without constant physical presence.

• Data Fragmentation: The complexity of centralizing data from various manufacturers and communication protocols.

• Security & Intellectual Property: Risks of unauthorized machine operation or the theft of proprietary PLC/HMI programming.

• Production Flexibility: The need to accurately manage and switch between complex parameter sets for diverse product lines (e.g., changing ingredient ratios for different types of bread).

**Solutions provided by FvDesigner**

• Remote Access: VNC Server enables remote screen monitoring and operation, while the FTP Server allows for remote access to HMI files.

• IoT Standardization: Native support for MQTT, OPC UA, and REST API bridges the gap between field devices and third-party cloud applications.

• Robust Security: Includes Multi-level user permissions, USB Security Keys for login, and Installment payment controls that lock machine operation until an authorization code is entered.

• Recipe Management: A system that groups parameters into Recipes, allowing operators to change multiple machine settings simultaneously with ease.

**Information Systems and Tools**

• FvDesigner: The core design environment for developing HMI projects.

• FvRT (PC Runtime): A tool that allows HMI projects to be executed on a PC for PLC communication.

• iAccess (FATEK Cloud): A cloud platform for secure remote maintenance, project updates, and monitoring.

• Modbus Gateway: Configures the HMI as a bridge between an upper-level SCADA system and multiple lower-level devices.

• Database Integration: Direct connectivity with MySQL and Microsoft SQL Server for data exchange and storage.

### Q2: Analyze and list the key five key components of an Information System (IS) using 5W1H method.

**1. Hardware (Where)**: P5 series HMI devices and Windows-based PCs (Windows 8/10/11) used for development and runtime.

**2. Software (What)**: FvDesigner (design tool) and FvRT (runtime environment) for controlling and monitoring industrial processes.

**3. Data (Why)**: Essential operational data including Recipes for production parameters, Alarms for safety, and Data Collection for long-term analysis.

**4. People (Who)**: System designers, authorized operators, and administrators who interact via secure multi-level login permissions.

**5. Process (How)**: The exchange of information through standard protocols like MQTT, OPC UA, and Modbus, synchronized with PLC devices to automate physical actions.

### Q3: Why did the designers include a physical electronic scale inside the digital box? How does this sensor integration (IoT) bridge the gap between abstract digital transactions and physical satisfaction?

While the manual does not explicitly mention a "charity digital box," it details the use of Recipes to manage physical material ratios (e.g., bread and cake ingredients). 
By integrating sensors (via PLC or IoT protocols like MQTT), abstract digital settings are converted into precise physical quantities. 
This integration ensures that digital transactions result in consistent physical outcomes, satisfying quality requirements and operational goals.

### Q4: The case claims a "positive outcome for all stakeholders." Beyond the charity receiving money, what is the specific value proposition for the Grocery Store hosting the device?

Beyond the primary function, a host (such as a grocery store) gains specific value through:

**• Data Analytics:** The system tracks usage and operational trends via the Data Collection feature, allowing the host to analyze performance.

**• Operational Security:** The Security management system ensures only authorized personnel can adjust settings, protecting the host's equipment.

**• Reduced Maintenance:** Remote monitoring via VNC Server or iAccess Cloud allows for troubleshooting without a physical technician on-site.

### Q5: The case study may be improved, what’s your top 3 recommendations?

**1. Implement Data Synchronization:** Use the Database Server integration (SQL) to backup and analyze historical data across multiple store locations centrally.

**2. Enhance Communication Security:** Use the PLC Transmission Encryption Tool to protect proprietary project files during remote updates to ensure system integrity.

**3. Utilize Dynamic Recipes:** Implement Recipe Selectors on the HMI interface to allow hosts to switch between different operational modes (or "charity campaigns") instantly and securely.

Does this analysis align with your goals, or would you like to dive deeper into how specific protocols like MQTT are configured?

### Q6: The RKD Group report notes that "New donor rates drop" while "Core donors" remain stable. How should this data influence the design of the "Attract Mode"? Should the machine focus on educating new people or recognizing repeat donors?

The "Screen Saver" (Attract Mode) in FvDesigner allows for "Custom Text" and specific "Fonts" to engage users. To prioritize repeat donors, the "Security" system can identify "Core Donors" using unique "User IDs" and "Passwords" to provide a personalized experience.

### Q7: Traditional models fail when data patterns change suddenly (e.g., natural disasters). How does the FoodRL framework use Reinforcement Learning to adapt to "Concept Drift" caused by events like hurricanes or wildfires?

While the software does not explicitly feature Reinforcement Learning, it uses "Scripts" to handle complex logic. These scripts can use "Logical Judgments" and "Arithmetic" to adapt the HMI's behavior to sudden external data changes.

### Q8: How could the real-time data collected by the "Small Donation" devices be fed into the AI system to create a more accurate, real-time map of community hunger, bypassing the need?

Real-time donation data is gathered using "Data Collection" groups. This information can be fed into an AI system by "Synchronizing" it to an SQL database or publishing it via "MQTT" and "REST API" protocols.

### Q9: According to the case study, why does $1 bought by a food bank equal 4-20 meals, whereas an individual's dollar only equals 1-2 meals? How does the system visualize this efficiency gap to change donor behavior?

Specific meal-to-dollar ratios can be managed as "Recipes" within the system. To change donor behavior, the system can visualize these efficiency gaps using "Pie Charts" or "Bar Graphs".

### Q10: How does the system utilize the "Attract Mode" (when idle) versus the "Feedback Screen" (post-donation) to create an emotional feedback loop? What specific visual elements are used to trigger empathy?

Designers use "Window Screen Displays" to provide immediate feedback after a donation. Specific visual elements to trigger empathy, such as photos or animations, are implemented using the "Image Library" and "GIF Display" features.





































