# Awesome CloudXR Resources 

A curated list of papers and open-source resources focused on CloudXR. If you have any additions or suggestions, feel free to contribute. Additional resources like blog posts, videos, etc. are also welcome.

## Table of contents
<br>

- [Architecture](#architecture)
- [Bisuness](#autonomous-driving)
- [CloudGaming](#cloudgaming)
- [CloudXR](#cloudxr)
- [Dataset](#dataset)
- [Latency](#latency)
- [Platform](#platform)
- [QoS](#qos)
- [QoE](#qoe)
- [Streaming](#streaming)
- [Virtulized](#virtulized)



<br>


- [Open Source Implementations](#open-source-implementations)
  * [Reference](#reference)

<br>

<br>

## Architecture

### 1. 3D Visualizations inWeb BasedEnvironment
**Authors**: 
<details span>
<summary><b>Abstract</b></summary>
This thesis presents a fully functional remote streaming web-based 3D visualization application, that will enable any device to render interactive 3D graphics in real-time. The application only requires a web browser to work and is not limited by the hardware/software and the physical size of the used device. Our application takes advantage of real-time communication technologies, like WebRTC, and multimedia frameworks, like GStreamer, to stream 3D content through the web browser. We also study the performance limitations of native rendering 3D content on mobile devices, by evaluating the number of objects various mobile devices are capable of rendering, concluding that mobile devices are less adequate to render a high number of polygons. In our experiments, the server completed the rendering, on average, 10% faster than our most powerful smartphone, and rendered 46 300 more objects.
</details>

 [📄 Paper](https://repositorio-aberto.up.pt/bitstream/10216/135828/2/489863.pdf) | [💻 Code ](https://github.com/Truvam/web-3d)

<br>

### 2. GamingAnywhere: an open cloud gaming system 
**Authors**: Chun-Ying Huang, Cheng-Hsin Hsu, Yu-Chun Chang, and Kuan-Ta Chen
<details span>
<summary><b>Abstract</b></summary>
GamingAnywhere is an open-source clouding gaming platform. In addition to its openness, we design GamingAnywhere for high extensibility, portability, and reconfigurability. GamingAnywhere currently supports Windows and Linux, and can be ported to other OS's including OS X and Android. Table 1 gives the latest supported OS's and versions. Our performance study demonstrates that GamingAnywhere achieves high responsiveness and video quality yet imposes low network traffic. The value of GamingAnywhere, however, is from its openness: researchers, service providers, and gamers may customize GamingAnywhere to meet their needs. This is not possible in other closed and proprietary cloud gaming platforms.
</details>

 [📄 Paper](https://gaminganywhere.org/doc.html) |  [🌐 Project Page](https://gaminganywhere.org/) | [💻 Code ](https://github.com/chunying/gaminganywhere)

<br>

### 3. GamingAnywhere: An Open-Source Cloud Gaming Testbed 
**Authors**: Chun-Ying Huang, De-Yu Chen, Cheng-Hsin Hsu, and Kuan-Ta Chen
<details span>
<summary><b>Abstract</b></summary>
While cloud gaming opens new business opportunity, it also poses tremendous challenges as the Internet only provides best-effort service and gamers are hard to please. Although researchers have various ideas to improve cloud gaming systems, existing cloud gaming systems are closed and proprietary, and cannot be used to evaluate these ideas. We present GamingAnywhere, the first open-source cloud gaming system, which is extensible, portable, and configurable. GamingAnywhere may be used by: (i) researchers and engineers to implement and test their new ideas, (ii) service providers to develop cloud gaming services, and (iii) gamers to set up private cloud gaming systems. Details on GamingAnywhere are given in this paper. We firmly believe GamingAnywhere will stimulate future studies on cloud gaming and real-time interactive distributed systems.
</details>

 [📄 Paper](https://gaminganywhere.org/doc.html) |  [🌐 Project Page](https://gaminganywhere.org/) | [💻 Code ](https://github.com/chunying/gaminganywhere)

<br>

### 4. GamingAnywhere—The First Open Source Cloud Gaming System
**Authors**: CHUN-YING HUANG, National Taiwan Ocean University, Taiwan KUAN-TA CHEN, Academia Sinica, Taiwan DE-YU CHEN, Academia Sinica, Taiwan HWAI-JUNG HSU, Academia Sinica, Taiwan CHENG-HSIN HSU, National Tsing Hua University, Taiwan
<details span>
<summary><b>Abstract</b></summary>
We present the first open source cloud gaming system, called GamingAnywhere. In addition to its openness, we design GamingAnywhere for high extensibility, portability, and reconfigurability. We implement GamingAnywhere on Windows, Linux, OS X, and Android. We conduct extensive experiments to evaluate the performance of GamingAnywhere. Our experimental results indicate that GamingAnywhere is efficient, scalable, adaptable to network conditions, and achieves high responsiveness and streaming quality. GamingAnywhere can be employed by the researchers, game developers, service providers, and end users for setting up cloud gaming testbeds, which, we believe, will stimulate more research innovations on cloud gaming systems and applications.
</details>

 [📄 Paper](https://gaminganywhere.org/doc.html) |  [🌐 Project Page](https://gaminganywhere.org/) | [💻 Code ](https://github.com/chunying/gaminganywhere)

<br>

### 5. LiveRender: A Cloud Gaming System Based on Compressed Graphics Streaming
**Authors**: Li Lin Xiaofei Liao  Guang Tan Hai Jin Xiaobin Yang Wei Zhang Bo Li
<details span>
<summary><b>Abstract</b></summary>
In cloud gaming systems, the game program runs at servers in the cloud, while clients access game services by sending input events to the servers and receiving game scenes via video streaming. In this paradigm, servers are responsible for all performance-intensive operations, and thus suffer from poor scalability. An alternative paradigm is calledgraphics streaming, in which graphics commands and data are offloaded to the clients for local rendering, thereby mitigating the server's burden and allowing more concurrent game sessions. Unfortunately, this approach is bandwidth consuming, due to large amounts of graphic commands and geometry data. In this paper, we present LiveRender, an open source gaming system that remedies the problem by implementing a suite of bandwidth optimization techniques including intra-frame compression, inter-frame compression, and caching, establishing what we call compressed graphics streaming. Experiments results show that the new approach is able to reduce bandwidth consumption by 52-73% compared to raw graphics streaming, with no perceptible difference in video quality and reduced response delay. Compared with the video streaming approach, LiveRender achieves a traffic reduction of 40-90% with even improved video quality and substantially smaller response delay, while enabling higher concurrency at the server.
</details>

 [📄 Paper](https://www.researchgate.net/publication/271769888_LiveRender_A_Cloud_Gaming_System_Based_on_Compressed_Graphics_Streaming) | [💻 Code ](https://github.com/llfjfz/LiveRender)

<br>

### 6. Nebula: Reliable Low-latency Video Transmission for Mobile Cloud Gaming
**Authors**: Ahmad Alhilal (1), Tristan Braud (1), Bo Han (2), Pan Hui (1) ((1) Hong Kong University of Science and Technology (2) George Mason University)
<details span>
<summary><b>Abstract</b></summary>
Mobile cloud gaming enables high-end games on constrained devices by streaming the game content from powerful servers through mobile networks. Mobile networks suffer from highly variable bandwidth, latency, and losses that affect the gaming experience. This paper introduces Nebula, an end-to-end cloud gaming framework to minimize the impact of network conditions on the user experience. Nebula relies on an end-to-end distortion model adapting the video source rate and the amount of frame-level redundancy based on the measured network conditions. As a result, it minimizes the motion-to-photon (MTP) latency while protecting the frames from losses. We fully implement Nebula and evaluate its performance against the state of the art techniques and latest research in realtime mobile cloud gaming transmission on a physical testbed over emulated and real wireless networks. Nebula consistently balances MTP latency (<140 ms) and visual quality (>31dB) even in highly variable environments. A user experiment confirms that Nebulamaximizes the user experience with high perceived video quality, playability, and low user load.
</details>

 [📄 Paper](https://arxiv.org/abs/2201.07738) 

<br>

### 7. Next Generation Mobile Cloud Gaming
**Authors**: Wei Cai, Victor C.M. Leung Min Chen
<details span>
<summary><b>Abstract</b></summary>
With the proliferation of smart mobile devices and broadband wireless networks, the mobile gaming market is rapidly expanding among younger generations due to its ubiquitous entertainment features. Cloud-based mobile computing is a promising technology to address the inherent restrictions of mobile devices, such as limited battery lifetime and computational capacity. In this work, we categorize the current approaches to cloud-based mobile gaming and explicitly define Mobile Cloud Gaming (MCG) 1. Based on its unique features, we propose a framework for next generation MCG systems. Open research issues for MCG are also discussed.
</details>

 [📄 Paper](https://www.semanticscholar.org/paper/Next-Generation-Mobile-Cloud-Gaming-Cai-Leung/2186e19c14861ca291e0e95cdbc48a418e7c5117) 

<br>

<br>

## Bisuness
- [Bisuness](https://Bisuness.html)

<br>

<br>

## CloudGaming
- [CloudGaming](https://CloudGaming.html)

<br>

<br>

## CloudXR
- [CloudXR](https://CloudXR.html)

<br>

<br>

## Dataset
- [Dataset](https://Dataset.html)

<br>

<br>

## Latency
- [Latency](https://Latency.html)

<br>

<br>

## Platform
- [Platform](https://Platform.html)

<br>

<br>

## QoS
- [QoS](https://QoS.html)

<br>

<br>

## QoE
- [QoE](https://QoE.html)

<br>

<br>

## Streaming
- [Streaming](https://Streaming.html)

<br>

<br>

## Virtulized
- [Virtulized](https://Virtulized.html)

<br>

<br>

## Open Source Implementations
- [Open Source Implementations](https://Virtulized.html)

<br>

## Credits

- Thanks to 
