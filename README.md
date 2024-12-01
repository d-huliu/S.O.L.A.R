

# S.O.L.A.R

## Seeing, Observing, Learning, And Remembering

![Cover](https://i.imgur.com/7MkG4m7.jpeg)
-----------------------------------------------------------------------------------------------------------------

# 🌟 SOLAR: Seeing, Observing, Learning, and Remembering through Augmented Reality 🌟

## 💭 Inspiration 💭

SOLAR was born out of the vision to empower individuals facing challenges of vision impairment, cognitive decline, and mobility limitations. In a world where over **2.2 billion people** live with some form of vision impairment, and diseases like Alzheimer’s affect millions, everyday tasks can become monumental hurdles. **SOLAR** aims to bridge the gap between these challenges and a life of independence, using augmented reality (AR) as a tool for empowerment.

Did you know?  
- Approximately **81% of vision-impaired individuals** are aged 50 and older.  
- Alzheimer's disease is the most common cause of dementia, impacting **55 million people worldwide** ([WHO](https://www.who.int/news-room/fact-sheets/detail/dementia)).  
- AR technology is expected to grow into a **$175 billion industry by 2030**, showing immense potential to transform healthcare and accessibility.

---

## ❓ What SOLAR Does ❓

**SOLAR** is an assistive AR application designed for the Microsoft HoloLens, revolutionizing accessibility for individuals with visual and cognitive challenges. It offers a suite of features aimed at enhancing everyday experiences:

- **Customizable Zoom**: Enables users to focus on specific objects or text with precision, making it easier to navigate their surroundings or read documents.  
- **Text-to-Speech Conversion**: Converts text from books, newspapers, TV captions, or even handwritten notes into spoken words, ensuring continuous access to information.  
- **Facial Recognition and Emotional Insights**: Identifies familiar faces, provides names for stored individuals, and estimates age, gender, and emotional states for others nearby.  
- **Emergency Assistance**: Integrated with Twilio, the app allows users to make instant emergency calls, providing a critical lifeline during urgent situations.

SOLAR is more than an app—it's a gateway to independence, tailored to the needs of those it serves.

---


## 🔧 How It Was Built 🔧

SOLAR was developed using a combination of advanced tools, APIs, and SDKs to deliver its rich feature set:

### Tools and Platforms:
- **Microsoft HoloLens**: The primary platform for AR development, leveraging its spatial mapping and real-world interaction capabilities.
- **Visual Studio 2017**: Used for development and debugging, ensuring seamless integration with the Universal Windows Platform (UWP).
- **Unity 2018**: Chosen for its robust support for 3D AR environments and compatibility with the Mixed Reality Toolkit.

### APIs and SDKs:
1. **Microsoft Azure Cognitive Services**:
   - **Computer Vision API**: Powers the text-to-speech feature by extracting text from scanned images or live video streams.
   - **Face API**: Used for facial recognition, providing detailed information such as age, gender, and emotional state in real-time.
   - **Speech Service**: Converts extracted text into spoken language with a natural-sounding voice, supporting multiple languages and accents.

2. **Mixed Reality Toolkit (MRTK)**:
   - Provides pre-built components for spatial mapping, hand tracking, and user interaction, allowing a seamless AR experience on the HoloLens.

3. **Windows 10 SDK**:
   - Used to build and deploy the application on the Universal Windows Platform, ensuring compatibility with the HoloLens hardware and OS.

### Development Process:
- The **Zoom Capability** was implemented using Unity’s camera manipulation tools and MRTK’s spatial understanding components, allowing smooth transitions and accurate scaling.
- The **Facial Recognition System** was built by integrating Azure’s Face API, which processes live video streams from the HoloLens camera.
- The **Text-to-Speech Functionality** relied on the Computer Vision API for text extraction, followed by the Speech Service to deliver auditory feedback.
---


## ⚓ Challenges We Faced ⚓

Developing **SOLAR** was a technically demanding project, particularly due to the constraints of working on legacy hardware and software platforms. The Microsoft HoloLens, while groundbreaking in its time, introduced a number of challenges that required creative problem-solving and meticulous optimization to deliver a robust and functional application.

### 1. **Legacy Hardware Constraints**
The HoloLens model we used was equipped with aging hardware, which significantly limited our development options:
- **USB 2.0 Bandwidth**: The restricted data transfer speeds severely impacted debugging, testing, and loading large assets onto the device. This created bottlenecks, particularly during iterative development cycles where rapid deployment is critical.
- **Wi-Fi 4 Connectivity**: The outdated networking capabilities of the HoloLens affected performance during cloud-based operations, such as retrieving data from Azure Cognitive Services in real time. This introduced latency and required us to pre-process as much data as possible locally.
- **Less than 1GB of Video Memory**: Rendering assets in real-time AR environments was a substantial challenge. The lack of sufficient VRAM forced us to optimize our models and textures aggressively, sacrificing graphical fidelity for performance.

### 2. **Software Limitations**
The limitations of the HoloLens hardware were compounded by restrictions in the software environment:
- **Unity 2018 vs. Unity 6**: We were locked into using Unity 2018 due to compatibility issues with the HoloLens' operating system. This meant we couldn't leverage the powerful features of modern Unity versions, such as enhanced rendering pipelines, improved AR foundations, and optimized workflows. Many cutting-edge features, like Shader Graph and modern visual effects, were unavailable, requiring manual implementation or workarounds.
- **Legacy .NET Framework**: The device's reliance on older versions of the .NET framework significantly restricted our ability to implement modern, efficient, and maintainable code. The lack of support for the newer IL2CPP (Intermediate Language to C++) framework was particularly challenging, as IL2CPP provides better performance, reduced memory usage, and compatibility with C++ libraries—features that would have been extremely beneficial for our computationally intensive tasks.


### 3. **Modern Development in a Legacy Ecosystem**
Working on legacy hardware and software created a disconnect between the tools we were accustomed to and those we were constrained to use:
- **Visual Studio Compatibility**: Developing with Visual Studio 2017, as opposed to newer versions, limited access to improved debugging tools, better performance profiling, and streamlined workflows.
- **Incompatibility with Modern Libraries**: Many third-party libraries and frameworks that would have enhanced development were incompatible with the legacy .NET framework, forcing us to build custom solutions for tasks such as asset loading, network optimization, and user interface design.

### 4. **Asset Optimization**
Given the hardware limitations, optimizing assets was one of the most significant challenges:
- Models and textures had to be simplified without compromising the user experience.
- Real-time rendering pipelines were stripped down to basic shaders and materials to meet performance constraints.
- Preloading assets became a critical strategy to avoid runtime bottlenecks, though it required careful memory management due to the limited resources.

---

### Overcoming These Challenges

Despite these obstacles, we successfully delivered **SOLAR** through:
- **Aggressive Optimization**: From code efficiency to asset management, every component of SOLAR was designed to run smoothly within the device's limitations.
- **Creative Problem-Solving**: Where modern tools and libraries were unavailable, we innovated to create custom solutions.
- **Iterative Testing and Feedback**: We leveraged a cycle of continuous testing, collecting real-world performance data, and refining the application to ensure it met both technical and user expectations.

The challenges we faced were immense, but they ultimately pushed us to think outside the box and develop a solution that not only works but excels within the constraints of legacy hardware. **SOLAR** stands as a testament to the power of adaptability, determination, and innovation in software development.

---

## 🏆 Accomplishments to Note 🏆

**SOLAR** has already demonstrated significant potential as a transformative assistive technology.  
Key achievements include:  
- **Improved Accessibility**: Enhanced the quality of life for individuals with visual and cognitive impairments by addressing daily challenges.  
- **Environmental Sustainability**: Efficiently optimized hardware usage on legacy devices, showcasing adaptability in constrained environments.  
- **Scalability**: Designed with modularity to ensure future iterations remain relevant across diverse user groups and technological advancements.

---

## ⏭ What’s Next for SOLAR? ⏭

The vision for SOLAR doesn’t stop here. Future developments aim to broaden its impact:  
- **Expanded Cognitive Tools**: Include memory training exercises and real-time reminders to assist individuals with dementia.  
- **Wearable Integration**: Develop versions compatible with lightweight AR glasses for easier adoption.  
- **Global Partnerships**: Collaborate with healthcare providers to distribute SOLAR to underserved communities.  
- **Government Adoption**: Partner with policymakers to establish SOLAR as part of national assistive technology programs.

**SOLAR** is not just a product—it's a movement to redefine how we think about accessibility and technology's role in empowerment.
