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

 Social Pain Points: One in seven Americans face food insecurity. Individual food donations are inefficient, providing only 1–2 meals per dollar, whereas food banks can provide 4–20 meals with the same amount.
 
• Solutions: A digital charity box in grocery stores that visualizes monetary donations as physical food, making the impact of small change tangible and satisfying for the donor.
• Information Systems: The system uses HMI (Human Machine Interface) software like FvDesigner to create interactive interfaces. It utilizes Data Collection to track donation totals and can use MQTT or REST API to sync data with charity servers.

### Q2: Analyze and list the key five key components of an Information System (IS) using 5W1H method.

**1. Who (People):** Donors, grocery store customers, and charity organizations.

**2. What (Software):** FvRT (Runtime) to operate the interactive donation interface designed in FvDesigner.

**3. Where (Hardware):** Industrial-grade HMI terminals (like the P5 series) housed in a physical donation box at grocery stores.

**4. Why (Data):** To convert abstract donation values into impact visualizations (e.g., meal counts) and track community contribution totals.

**5. How (Process):** Using Scripts to calculate food equivalents and FTP/MQTT protocols to transmit transaction data securely [27, 28, 4.5].

### Q3: Why did the designers include a physical electronic scale inside the digital box? How does this sensor integration (IoT) bridge the gap between abstract digital transactions and physical satisfaction?

While the transcript focuses on "visualizations", the inclusion of a physical electronic scale (integrated via a PLC or IoT service) bridges the gap by providing a sensory "fun interaction". This turns an abstract digital transaction into a physical experience, where the donor sees a tangible representation of weight or volume, leading to higher "physical satisfaction" that their money was well spent.

### Q4: The case claims a "positive outcome for all stakeholders." Beyond the charity receiving money, what is the specific value proposition for the Grocery Store hosting the device?

Beyond charity, the store benefits by:

**• Community Engagement:** Facilitating a "fun interaction" that increases customer time-on-site.
**• Brand Image:** It fosters a "positive view of their business" by aligning the store with local social causes.
**• Operational Insights:** Using Operation Log or Data Collection features to see peak donation times, which can correlate with customer traffic data.

### Q5: The case study may be improved, what’s your top 3 recommendations?

**1. Dynamic Impact Updates:** Use REST API or MQTT to pull real-time data from food banks, showing donors exactly which community pantry their specific dollar is currently stocking.

**2. Donor Recognition:** Use Security/User Management (via RFID or User ID) to recognize "Core Donors," allowing the machine to display a "Welcome Back" message or cumulative impact history.

**3. Logistics Integration:** Use SQL Database connectivity to sync donation data across multiple store locations, allowing the charity to optimize food distribution logistics based on where funds are being raised.

### Q6: The RKD Group report notes that "New donor rates drop" while "Core donors" remain stable. How should this data influence the design of the "Attract Mode"? Should the machine focus on educating new people or recognizing repeat donors?

The "Attract Mode" (initial looping screens) focuses on attracting new donors by showing images of the charity's impact on the community and side-by-side comparisons of food purchasing power. While HMI software supports identifying repeat users via "User IDs", the transcript emphasizes educating new donors by showing the "faces of those in need" to trigger empathy.

### Q7: Traditional models fail when data patterns change suddenly (e.g., natural disasters). How does the FoodRL framework use Reinforcement Learning to adapt to "Concept Drift" caused by events like hurricanes or wildfires?

While the provided snippets do not mention the "FoodRL" framework specifically, the FvDesigner system can technically adapt to sudden data changes through Scripts. These allow for "Logic judgments" (if/else) and arithmetic operations, enabling the HMI to change behavior based on external inputs or disaster-related variables.

### Q8: How could the real-time data collected by the "Small Donation" devices be fed into the AI system to create a more accurate, real-time map of community hunger, bypassing the need?

Real-time data from donation devices can be published to a central system using MQTT or REST API protocols. By publishing data to a central "Broker" or synchronizing with an SQL database, the system can aggregate individual donation points into a real-time hunger map for community analysis.

### Q9: According to the case study, why does $1 bought by a food bank equal 4-20 meals, whereas an individual's dollar only equals 1-2 meals? How does the system visualize this efficiency gap to change donor behavior?

A food bank can buy 4-20 meals per $1, whereas an individual buys only 1-2 meals because charities have bulk purchasing power and wholesale efficiency. The system visualizes this gap using a side-by-side comparison on the screen, showing the donor that their monetary gift provides significantly more food than a physical donation.

### Q10: How does the system utilize the "Attract Mode" (when idle) versus the "Feedback Screen" (post-donation) to create an emotional feedback loop? What specific visual elements are used to trigger empathy?

The system creates an emotional loop by alternating between two modes:
• **Attract Mode (Idle):** Uses "faces of those in need" to trigger empathy and loops "images of impact" to show the charity's effectiveness.
• **Feedback Screen (Post-Donation):** Surprises the donor with "visualizations of different foods" purchased with their specific contribution. This ensures the donor walks away "satisfied that their money was well spent".





































