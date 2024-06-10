# Awesome CloudXR / CloudGaming Resources 

A curated list of papers and open-source resources focused on CloudXR. If you have any additions or suggestions, feel free to contribute. Additional resources like blog posts, videos, etc. are also welcome.

## Table of contents
<br>

- [Architecture](#architecture)
- [Business](#business)
- [CloudGaming](#cloudgaming)
- [CloudXR](#cloudxr)
- [Dataset](#dataset)
- [Edge 5G](#edge-5g)
- [Latency](#latency)
- [QoE](#qoe)
- [QoS](#qos)
- [Streaming](#streaming)
- [Survey](#survey)
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

### 2. Cloud gaming: architecture and performance
**Authors**: R. Shea, Jiangchuan Liu, E. Ngai, Yong Cui
<details span>
<summary><b>Abstract</b></summary>
Recent advances in cloud technology have turned the idea of Cloud Gaming into a reality. Cloud Gaming, in its simplest form, renders an interactive gaming application remotely in the cloud and streams the scenes as a video sequence back to the player over the Internet. This is an advantage for less powerful computational devices that are otherwise incapable of running high quality games. Such industrial pioneers as Onlive and Gaikai have seen success in the market with large user bases. In this article, we conduct a systematic analysis of state-of-theart cloud gaming platforms, and highlight the uniqueness of their framework design. We also measure their real world performance with different types of games, for both interaction latency and streaming quality, revealing critical challenges toward the widespread deployment of Cloud Gaming.
</details>

 [📄 Paper](https://www.sfu.ca/~rws1/papers/Cloud-Gaming-Architecture-and-Performance.pdf) 

<br>

### 3. GamingAnywhere: an open cloud gaming system 
**Authors**: Chun-Ying Huang, Cheng-Hsin Hsu, Yu-Chun Chang, and Kuan-Ta Chen
<details span>
<summary><b>Abstract</b></summary>
GamingAnywhere is an open-source clouding gaming platform. In addition to its openness, we design GamingAnywhere for high extensibility, portability, and reconfigurability. GamingAnywhere currently supports Windows and Linux, and can be ported to other OS's including OS X and Android. Table 1 gives the latest supported OS's and versions. Our performance study demonstrates that GamingAnywhere achieves high responsiveness and video quality yet imposes low network traffic. The value of GamingAnywhere, however, is from its openness: researchers, service providers, and gamers may customize GamingAnywhere to meet their needs. This is not possible in other closed and proprietary cloud gaming platforms.
</details>

 [📄 Paper](https://gaminganywhere.org/doc.html) |  [🌐 Project Page](https://gaminganywhere.org/) | [💻 Code ](https://github.com/chunying/gaminganywhere)

<br>

### 4. GamingAnywhere: An Open-Source Cloud Gaming Testbed 
**Authors**: Chun-Ying Huang, De-Yu Chen, Cheng-Hsin Hsu, and Kuan-Ta Chen
<details span>
<summary><b>Abstract</b></summary>
While cloud gaming opens new business opportunity, it also poses tremendous challenges as the Internet only provides best-effort service and gamers are hard to please. Although researchers have various ideas to improve cloud gaming systems, existing cloud gaming systems are closed and proprietary, and cannot be used to evaluate these ideas. We present GamingAnywhere, the first open-source cloud gaming system, which is extensible, portable, and configurable. GamingAnywhere may be used by: (i) researchers and engineers to implement and test their new ideas, (ii) service providers to develop cloud gaming services, and (iii) gamers to set up private cloud gaming systems. Details on GamingAnywhere are given in this paper. We firmly believe GamingAnywhere will stimulate future studies on cloud gaming and real-time interactive distributed systems.
</details>

 [📄 Paper](https://gaminganywhere.org/doc.html) |  [🌐 Project Page](https://gaminganywhere.org/) | [💻 Code ](https://github.com/chunying/gaminganywhere)

<br>

### 5. GamingAnywhere—The First Open Source Cloud Gaming System
**Authors**: CHUN-YING HUANG, National Taiwan Ocean University, Taiwan KUAN-TA CHEN, Academia Sinica, Taiwan DE-YU CHEN, Academia Sinica, Taiwan HWAI-JUNG HSU, Academia Sinica, Taiwan CHENG-HSIN HSU, National Tsing Hua University, Taiwan
<details span>
<summary><b>Abstract</b></summary>
We present the first open source cloud gaming system, called GamingAnywhere. In addition to its openness, we design GamingAnywhere for high extensibility, portability, and reconfigurability. We implement GamingAnywhere on Windows, Linux, OS X, and Android. We conduct extensive experiments to evaluate the performance of GamingAnywhere. Our experimental results indicate that GamingAnywhere is efficient, scalable, adaptable to network conditions, and achieves high responsiveness and streaming quality. GamingAnywhere can be employed by the researchers, game developers, service providers, and end users for setting up cloud gaming testbeds, which, we believe, will stimulate more research innovations on cloud gaming systems and applications.
</details>

 [📄 Paper](https://gaminganywhere.org/doc.html) |  [🌐 Project Page](https://gaminganywhere.org/) | [💻 Code ](https://github.com/chunying/gaminganywhere)

<br>

### 6. LiveRender: A Cloud Gaming System Based on Compressed Graphics Streaming
**Authors**: Li Lin Xiaofei Liao  Guang Tan Hai Jin Xiaobin Yang Wei Zhang Bo Li
<details span>
<summary><b>Abstract</b></summary>
In cloud gaming systems, the game program runs at servers in the cloud, while clients access game services by sending input events to the servers and receiving game scenes via video streaming. In this paradigm, servers are responsible for all performance-intensive operations, and thus suffer from poor scalability. An alternative paradigm is calledgraphics streaming, in which graphics commands and data are offloaded to the clients for local rendering, thereby mitigating the server's burden and allowing more concurrent game sessions. Unfortunately, this approach is bandwidth consuming, due to large amounts of graphic commands and geometry data. In this paper, we present LiveRender, an open source gaming system that remedies the problem by implementing a suite of bandwidth optimization techniques including intra-frame compression, inter-frame compression, and caching, establishing what we call compressed graphics streaming. Experiments results show that the new approach is able to reduce bandwidth consumption by 52-73% compared to raw graphics streaming, with no perceptible difference in video quality and reduced response delay. Compared with the video streaming approach, LiveRender achieves a traffic reduction of 40-90% with even improved video quality and substantially smaller response delay, while enabling higher concurrency at the server.
</details>

 [📄 Paper](https://www.researchgate.net/publication/271769888_LiveRender_A_Cloud_Gaming_System_Based_on_Compressed_Graphics_Streaming) | [💻 Code ](https://github.com/llfjfz/LiveRender)

<br>

### 7. Nebula: Reliable Low-latency Video Transmission for Mobile Cloud Gaming
**Authors**: Ahmad Alhilal (1), Tristan Braud (1), Bo Han (2), Pan Hui (1) ((1) Hong Kong University of Science and Technology (2) George Mason University)
<details span>
<summary><b>Abstract</b></summary>
Mobile cloud gaming enables high-end games on constrained devices by streaming the game content from powerful servers through mobile networks. Mobile networks suffer from highly variable bandwidth, latency, and losses that affect the gaming experience. This paper introduces Nebula, an end-to-end cloud gaming framework to minimize the impact of network conditions on the user experience. Nebula relies on an end-to-end distortion model adapting the video source rate and the amount of frame-level redundancy based on the measured network conditions. As a result, it minimizes the motion-to-photon (MTP) latency while protecting the frames from losses. We fully implement Nebula and evaluate its performance against the state of the art techniques and latest research in realtime mobile cloud gaming transmission on a physical testbed over emulated and real wireless networks. Nebula consistently balances MTP latency (<140 ms) and visual quality (>31dB) even in highly variable environments. A user experiment confirms that Nebulamaximizes the user experience with high perceived video quality, playability, and low user load.
</details>

 [📄 Paper](https://arxiv.org/abs/2201.07738) 

<br>

### 8. Next Generation Mobile Cloud Gaming
**Authors**: Wei Cai, Victor C.M. Leung Min Chen
<details span>
<summary><b>Abstract</b></summary>
With the proliferation of smart mobile devices and broadband wireless networks, the mobile gaming market is rapidly expanding among younger generations due to its ubiquitous entertainment features. Cloud-based mobile computing is a promising technology to address the inherent restrictions of mobile devices, such as limited battery lifetime and computational capacity. In this work, we categorize the current approaches to cloud-based mobile gaming and explicitly define Mobile Cloud Gaming (MCG) 1. Based on its unique features, we propose a framework for next generation MCG systems. Open research issues for MCG are also discussed.
</details>

 [📄 Paper](https://www.semanticscholar.org/paper/Next-Generation-Mobile-Cloud-Gaming-Cai-Leung/2186e19c14861ca291e0e95cdbc48a418e7c5117) 

<br>

<br>

## Business

<br>

### 1. Cloud Pricing Models: Taxonomy, Survey, and Interdisciplinary Challenges
**Authors**: CAESAR WU, RAJKUMAR BUYYA, and KOTAGIRI RAMAMOHANARAO
<details span>
<summary><b>Abstract</b></summary>
This article provides a systematic review of cloud pricing in an interdisciplinary approach. It examines many historical cases of pricing in practice and tracks down multiple roots of pricing in research. The aim is to help both cloud service provider (CSP) and cloud customers to capture the essence of cloud pricing when they need to make a critical decision either to achieve competitive advantages or to manage cloud resource effectively. Currently, the number of available pricing schemes in the cloud market is overwhelming. It is an intricate issue to understand these schemes and associated pricing models clearly due to involving several domains of knowledge, such as cloud technologies, microeconomics, operations research, and value theory. Some earlier studies have introduced this topic unsystematically. Their approaches inevitably lead to much confusion for many cloud decision-makers. To address their weaknesses, we present a comprehensive taxonomy of cloud pricing, which is driven by a framework of three fundamental pricing strategies that are built on nine cloud pricing categories. These categories can be further mapped onto a total of 60 pricing models. Many of the pricing models have been already adopted by CSPs. Others have been widespread across in other industries. We give descriptions of these model categories and highlight both advantages and disadvantages. Moreover, this article offers an extensive survey of many cloud pricing models that were proposed by many researchers during the past decade. Based on the survey, we identify four trends of cloud pricing and the general direction, which is moving from intrinsic value per physical box to extrinsic value per serverless sandbox. We conclude that hyper-converged cloud resources pool supported by cloud orchestration, virtual machine, Open Application Programming Interface, and serverless sandbox will drive the future of cloud pricing.
</details>

 [📄 Paper](https://www.academia.edu/download/91269318/CloudPricingModels-Taxonomy.pdf) 

<br>

### 2. Developing Cloud Business Models: A Case Study on Cloud Gaming
**Authors**: Arto Ojala and Pasi Tyrväinen, University of Jyväskylä
<details span>
<summary><b>Abstract</b></summary>
Cloud computing offers new ways for firms to operate in the global market so that even small firms can compete in markets traditionally dominated by multinational corporations. A case study considers how, over ten years, a small firm developed a successful business model to compete in computer gaming.
</details>

 [📄 Paper](https://jyx.jyu.fi/bitstream/handle/123456789/36950/1/developing%20cloud%20business%20models%20a%20case%20study%20on%20cloud%20gaming.pdf) 

<br>

<br>

## CloudGaming

### 1. A Cost-Efficient Cloud Gaming System at Scale
**Authors**: 
<details span> Yiling Xu; Qiu Shen; Xin Li; Zhan Ma
<summary><b>Abstract</b></summary>
This article proposes a transparent gaming (TG) cloud system that allows users to play any popular high-end desktop game on the fly over the Internet. Toward this goal, we have introduced the TG-SHARE technology to share the underlying hardware capabilities, particularly for the GPU and the dedicated compression acceleration unit (XCODER). TG-SHARE utilizes offthe- shelf consumer GPUs without resorting to expensive proprietary GPU virtualization technology (e.g., GRID from NVIDIA). XCODER adapts the compression based on the network dynamics, learned gaming behaviors, and hardware resources to significantly reduce bandwidth consumption. Google's webRTC protocol is integrated to offer real-time interaction and ubiquitous access from heterogeneous devices. Compared to the existing cloud gaming vendor using the GRID technology, our TG-SHARE not only reduces the expense per user (i.e., 75 percent hardware cost reduction, 20-40 percent network cost reduction), but also improves the quality of experience with higher rate of frames per second (i.e., 2 x FPS).
</details>

 [📄 Paper](https://www.semanticscholar.org/paper/A-Cost-Efficient-Cloud-Gaming-System-at-Scale-Xu-Shen/e6e00827374517a1795a405cdf5a838a09f8b4db)

<br>

### 2. An empirical study of cloud gaming
**Authors**: 
<details span> M. Manzano∗, J. A. Hern ́andez†, M. Urue ̃na†, E. Calle∗
<summary><b>Abstract</b></summary>
Online gaming connects players from all over the world together for fun and entertainment, and has been regarded as one of the most profitable and popular Internet services. Besides, there is a growing trend towards moving local applications to remote data centers: this is often referred to as the cloud. With the purpose of studying the impact of Cloud Gaming on the access network load, in this paper we carry out an empirical network traffic analysis of two well-known cloud gaming platforms: On-Live and Gaikai. Traffic traces have been collected and analysed from five different games of both platforms. Cloud gaming has been observed to be remarkably different from traditional online gaming in terms of network load and traffic characteristics. Moreover, the traces have revealed similarities between the two platforms regarding the packet size distribution, and differences concerning the packet inter-arrival times. However, each platform shows a similar traffic pattern for most of the games it serves. Nonetheless, the racing and shooter games considered in this work demand more bandwidth than other game-genres.
</details>

 [📄 Paper](https://www.semanticscholar.org/paper/An-empirical-study-of-Cloud-Gaming-Manzano-Hern%C3%A1ndez/448a31ff7f9c599d4956e1676adc47e388a6d59b) 

<br>

### 3. Are all games equally cloud-gaming-friendly?: an electromyographic approach
**Authors**: 
<details span>
<summary><b>Abstract</b></summary>
Cloud gaming now makes any computer game playable on a thin client without the previous worries and frustrations about the hardware requirements. It frees players from the need to frequently upgrade their computers as they can now play games that are hosted on remote servers with a broadband Internet connection and a thin client. However, cloud games are intrinsically more susceptible to latency than online games because game graphics are rendered on cloud servers and thin clients do not possess game state information that is required by delay compensation techniques. In this paper, we investigate how the response latency in cloud gaming would affect users' experience and how the impact of latency on players' experience varies among different games. We show that not all games are equally friendly to cloud gaming. That is, the same degree of latency may have very different impacts on a game's quality of experience depending on the game's real-time strictness. We thus develop a model that can predict a game's real-time strictness based on the rate of players' inputs and the game screen dynamics. The model can be used to simultaneously enhance players' gaming experience and optimize the operation cost of data centers.
</details>


<br>

### 4. Cloud Computing's Killer App: Gaming
**Authors**: 
<details span>
<summary><b>Abstract</b></summary>
AmD's proposed online supercomputer willhandle gaming graphics so your cellphonewon't have to
</details>

<br>

### 5. Cloud Gaming Demystified: An Introduction to the Legal Implications of Cloud-Based Video Games
**Authors**: 
<details span>Mitchell Longan,* Gaetano Dimita,**
<summary><b>Abstract</b></summary>
In this paper, we set out to 'demystify' cloud-based videogaming andits legal implications. We do this in two stages. First, we offer adescriptive analysis of the videogame sector, including relevantmarkets and supply chains. We explain the basics of cloud computingtechnology, traditional videogame technology, and how the twoconverge in cloud-based videogame ecosystems. We also analyzemarket structures for both the cloud and video game industries, aswell as relevant supply chains, in order to understand how thesemarkets will overlap. Based on these analyses, we make predictionsabout how the cloud gaming market will be structured, including abreakdown of three separate models for cloud gaming services: the'layered' model of Gaming-as-a-Service ('GaaS'), the 'integrated'model of GaaS, and the 'consumer infrastructure-as-a-service' model.Finally, we use these three models to analyze how certain intellectualproperty rights, contractual rights, and regulatory issues will developin this novel environment for videogame distribution and access.
</details>

 [📄 Paper](https://repository.law.umich.edu/mtlr/vol29/iss1/2/) 

<br>

### 6. Cloud Gaming Platforms: Their impact on the future of the video game industry
**Authors**: 
<details span>
<summary><b>Abstract</b></summary>
How will cloud gaming platforms affect the future progression of the video game industry? Inthis thesis, I analyze how the implementation and further progression of cloud gaming platformswill affect the video game industry in the future, through exploratory research. By using deskresearch and historical data, this thesis aims to express the reshaping that the video gameindustry has been through from its invention to its current state, as well as its future prospects.Based on the framework of Porter's five forces and Suarez' battle for technological dominance, Ihave used a combination of both frameworks firstly to analyze the current state of the videogame industry, as well as, the changes that will occur with the implementation of cloud gamingplatforms. Secondly, the framework is then used to analyze how the different cloud technology,and the companies behind them, compete throughout its lifecycle to gain dominance in theindustry. Porter's five forces gives me the indication that the threat level in the industry willremain the same after the implementation of cloud gaming platforms. While Suarez' battle fortechnological dominance shows that cloud gaming platforms are still in a too early phase toaccurately gauge where it is headed. Aside from these two frameworks, there have also beenconducted semi-structured expert interviews with software developers to get a better grasp ofhow the industry is reaction to cloud gaming platforms. By using the results of these frameworksand the expert interviews, I will then discuss three possible scenarios that could be the futureoutcome of cloud gaming platforms. A key finding in the study indicates that cloud gamingplatforms have a promising future ahead where more companies are investing into them. Thisthesis contributes to existing literature by providing an overview of the current state and anoutline of future prospect for cloud gaming platforms.
</details>

 [📄 Paper](https://oda.oslomet.no/oda-xmlui/bitstream/handle/11250/2824063/Le_TriTue.pdf?sequence=3) 

<br>

### 7. CloudyGame: Enabling cloud gaming on the edge with dynamic asset streaming and shared game instances
**Authors**: A. Bhojan, Siang Ping Ng, J. Ng, Wei Tsang Ooi
<details span>
<summary><b>Abstract</b></summary>
Cloud gaming has emerged as a new computer game delivery paradigm that promises gaming anywhere, anytime, on any device, by running the computer game on a cloud server and streaming the rendered frames to users. To fulfill its promises, a cloud gaming provider must face three main challenges: reducing the interaction latency, reducing the cloud infrastructure cost, and reducing the network bandwidth demand. One way to reduce interaction latency is to run the game on the edge instead of the cloud. This introduces two additional challenges due to the limited resources available on the edge servers. First, there is a high initialization cost to install a game on the edge server if the game that a player wishes to play is not already installed. Second, an edge server typically has limited computing resources compared to the servers in the cloud. In this work, we address these two issues by proposing CloudyGame, a new software architecture for developing computer games, in which (i) resources are more efficiently shared and managed between different playing instances, and (ii) game assets are streamed on-demand to reduce the initialization cost. CloudyGame is implemented with a popular game engine, and thus any game built on the engine supports CloudyGame out of the box. Our evaluation shows that a game running on CloudyGame architecture needs 70–80% less RAM, VRAM, and CPU than a game using conventional architecture when running with four players. Furthermore, the game asset streaming system reduces the game's initial loading time by 70%. Hence, our cloud gaming architecture is highly scalable and economically deployable to the edge. Further, due to a reduction in resource usage, the CloudyGame architecture would benefit games running in the cloud as well.
</details>

 [📄 Paper](https://www.researchgate.net/publication/343919149_CloudyGame_Enabling_cloud_gaming_on_the_edge_with_dynamic_asset_streaming_and_shared_game_instances) 

<br>

### 8. Edge Gaming: A Greening Perspective
**Authors**: Francesco Spinellia,b,∗, Antonio Bazco-Noguerasa, Vincenzo Mancusoa
<details span>
<summary><b>Abstract</b></summary>
We tackle the problem of how to support gaming at the edge of the cellular network. The reduced latency and higher bandwidth that the edge enjoys with respect to cloud-based solutions implies that transferring cloud-based games to the edge could be a premium service for end-users. The goal of this work is to design a scheme compatible with MEC and network slicing principles of 5G and beyond, and which maximizes the utility of a service/infrastructure provider with time-varying edge node capacities due to the access to intermittent renewable energy. We formulate a multi -dimensional integer linear programming problem, proving that it is NP-hard in the strong sense. We prove that our problem is sub-modular and propose an efficient heuristic, GREENING, which considers the allocation of gaming sessions and their migration. For the mentioned scenario, we analyze a wide variety of realistic configurations at the edge, studying how the performance depends on i) whether the games have a static or dynamic workload, ii) the distribution of renewable energy through nodes and time, or iii) the topology of the edge network. Through simulations, we show that our heuristic achieves performance close to that achieved by solving the NP-hard optimization problem, except with extremely lower complexity, and performs up to 25% better than state-of-the-art algorithms.
</details>

 [📄 Paper](https://dspace.networks.imdea.org/bitstream/handle/20.500.12761/1598/Edge_Gaming__a_Greening_Perspective_CAMERA_READY.pdf?sequence=1) 

<br>

### 9. Rendering Server Allocation for MMORPG Players in Cloud Gaming
**Authors**: Iryanto Jaya, PictureWentong Cai, PictureYusen Li
<details span>
<summary><b>Abstract</b></summary>
Cloud gaming services enable users with heterogeneous device capabilities to get access to game titles with hardware demanding specifications. While visual quality requirements are to be satisfied by the cloud rendering servers, latency is one of the major problems which arises as most of the tasks are offloaded remotely. Cloud gaming players must experience latency below a certain acceptable limit for the game to be responsive with playable visual quality under limited bandwidth capacity. Playing multiplayer games in the cloud needs to cater for player interactions and their commonality especially if they are playing in the same virtual space. The main characteristic of cloud gaming is that the whole rendering pipeline occurs in the cloud; therefore, rendering optimization by reusing common information across players is possible by taking advantage of multi-view rendering. In this paper, we propose a cloud gaming architecture for MMORPGs which involves hundreds of players as well as online optimization heuristic algorithms on rendering server allocations in order to minimize rendering server rental cost from game provider's point of view. In addition, we also compare the performance of those online heuristics with an offline lower bound in order to observe the scalability of the online scenario.
</details>

 [📄 Paper](https://jnamaral.github.io/icpp20/slides/Jaya_Rendering.pdf) 

<br>

### 10. The Future of Cloud Gaming [Point of View]
**Authors**: Wei Cai, R. Shea, Chun-Ying Huang, Kuan-Ta Chen, Jiangchuan Liu, Victor C. M. Leung, Cheng-Hsin Hsu
<details span>
<summary><b>Abstract</b></summary>
In the late 2000s, several startups including OnLive [7] and GaiKai [8] started to offer cloud gaming services. Cloud gaming, as illustrated in Fig. 1, refers to the technologies that offload parts of game software from traditional game consoles or personal computers (PCs) to powerful and elastic cloud infrastructures. Cloud gaming makes perfect sense to: 1) gamers, who otherwise have to constantly upgrade their consoles or PCs, which is certainly no fun and costly; 2) cloud service providers, who can sell the already-deployed and idling cloud resources to support the cutting-edge games that are extremely resource hungry; and 3) game developers, who no longer need to spend months to port their games to different platforms. As such, cloud gaming has attracted significant attention from both academia and industry. Initially, given the limited scales of these startups, people were not sure whether cloud gaming could be commercially successful. A fundamental question that came to people, inside and outside the gaming circle, was: Will the three dominating console manufacturers, Microsoft, Nintendo, and Sony, be willing to give up their margin of selling the game consoles? The answer was initially unclear, and many suspected that these console manufacturers would be more than happy to kill cloud gaming in order to remain profitable. The opposite actually happened: Sony acquired GaiKai in 2012 for $380 million, announced the new service PlayStation Now (PS Now) in early 2014, and brought PS Now to parts of the world in 2015. Using PS Now, Sony allows their customers to play hundreds of PlayStation 3 (PS3) games on the latest PlayStation 4 (PS4) consoles without porting the games. Sony has also unveiled a plan to: 1) allow gamers to use other PlayStation consoles and smart TV to access PS Now; and 2) include game titles developed for other generations of PlayStations on PS Now. The emerging PS Now service indicates that cloud gaming has great potential to become the next-generation, universal computer gaming platform. Offering high-quality cloud gaming experience with the remote cloud through the public Internet, however, is no easy task. Current cloud gaming services have leveraged real-time video streaming technologies that have a long history of development. They share certain common characteristics, including high bandwidth demand and real-time constraints. Yet the demands of gaming are often higher than live or on-demand video streaming. Certain cloud gaming services dictate a network bandwidth of about 5 Mb/s for smooth gaming experience, which Corresponding author: Jiangchuan Liu (e-mail: jcliu@sfu.ca).
</details>

 [📄 Paper](https://www.cs.sfu.ca/~jcliu/Papers/CloudGaming-ProcIEEE-2016.pdf)

<br>

 ### 11. The Server Allocation Problem for Session-Based Multiplayer Cloud Gaming
**Authors**: Yunhua Deng, Yusen Li, Ronald Seet, Xueyan Tang, Wentong Cai
<details span>
<summary><b>Abstract</b></summary>
Advances in cloud computing and GPU virtualization are allowing the game industry to move into a cloud gaming era. In this paper, we consider multiplayer cloud gaming (MCG), which is the natural integration of multiplayer online gaming and cloud gaming paradigms. With MCG, a game server and a set of rendering servers for the players need to be located and launched in the clouds for each game session. We formulate an MCG server allocation problem with the objective of minimizing the total server rental and bandwidth cost charged by the cloud to support an MCG session. The MCG server allocation problem is hard to solve optimally. We propose several efficient heuristics to address the problem and carry out theoretical analysis for the proposed hill-climbing algorithm. We conduct extensive experiments using real Internet latency and cloud pricing datasets to evaluate the effectiveness of our proposed algorithms as well as several alternatives. Experimental results show that our best algorithm can achieve near-optimal cost under real-time latency constraints.
</details>

 [📄 Paper](https://dr.ntu.edu.sg/bitstream/10356/90123/1/The%20Server%20Allocation%20Problem%20for%20Session-Based%20Multiplayer%20Cloud%20Gaming.pdf) 

<br>

<br>

## CloudXR

 ### 1. A Robust Display Delay Compensation Technique Considering User’s Head Motion Direction for Cloud XR
**Authors**: Tatsuya Kobayashi, Tomoaki Konno, H. Kato
<details span>
<summary><b>Abstract</b></summary>
Conventionally, it has been difficult to realize both photorealistic and geometrically consistent 3DCG rendering on head mounted displays (HMDs), due to the trade-off between rendering quality and low motion-to-photon latency (M2PL). In order to solve this problem, we propose a novel rendering framework, where the server renders RGB-D images of a 3D model with the optimally arranged rendering viewpoints, and the client HMD realizes geometric compensation of M2PL by employing depth image based rendering (DIBR). Experiments with real smart glasses show that the proposed method can display binocular images closer to the ground truth than the conventional approaches.
</details>

<br>

 ### 2. CloudVR - Secure, Fast and Distributed Virtual Reality Solutions
**Authors**: Leon Koster
<details span>
<summary><b>Abstract</b></summary>
The graduations goal was to find out: "Which Technology stack(s) for building a cloud Virtual Reality (VR) streaming application satisfies the clients demands (low latency, security, QoE) best ? ". The chosen technology stack is NVIDIA's CloudXR SDK deployed on an Microsoft Azure Server, since it was the only feasible way to provide a working prototype for the client within the project timeframe. The report includes the neccessary theoretical knowledge, the decision making progress behind the prototype, implementation and testing of the prototype and implications of the results of the tests. The prototype in it's final set up had an individual frame latency that was only 1-2 ms higher than the researched barrier of 20ms and fulfilled security demands.
</details>

 [📄 Paper](https://github.com/Aptanaa/CloudVR-Thesis) 

<br>


 ### 3. CloudVR: Cloud Accelerated Interactive Mobile Virtual Reality
**Authors**: Teemu Kämäräinen, M. Siekkinen, Jukka Eerikäinen, Antti Ylä-Jääski
<details span>
<summary><b>Abstract</b></summary>
High quality immersive Virtual Reality experience currently requires a PC setup with cable connected head mounted display, which is expensive and restricts user mobility. This paper presents CloudVR which is a system for cloud accelerated interactive mobile VR. It is designed to provide short rotation and interaction latencies through panoramic rendering and dynamic object placement. CloudVR also includes rendering optimizations to reduce serverside computational load and bandwidth requirements between the server and client. Performance measurements with a CloudVR prototype suggest that the optimizations make it possible to double the server's framerate and halve the amount of bandwidth required and that small objects can be quickly moved at run time to client device for rendering to provide shorter interaction latency. A smallscale user study indicates that CloudVR users do not notice small network latencies (20ms) and even much longer ones (100-200ms) become non-trivial to detect when they do not affect the interaction with objects. Finally, we present a design of CloudVR extension to multi-user scenarios.
</details>

 [📄 Paper](https://www.researchgate.net/publication/328375148_CloudVR_Cloud_Accelerated_Interactive_Mobile_Virtual_Reality) 

<br>


 ### 4. Cutting the Cord: Designing a High-quality Untethered VR System with Low Latency Remote Rendering
**Authors**: Luyang Liu, Ruiguang Zhong, Wuyang Zhang, Yunxin Liu, Jiansong Zhang, Lintao Zhang, M. Gruteser
<details span>
<summary><b>Abstract</b></summary>
This paper introduces an end-to-end untethered VR system design and open platform that can meet virtual reality latency and quality requirements at 4K resolution over a wireless link. High-quality VR systems generate graphics data at a data rate much higher than those supported by existing wireless-communication products such as Wi-Fi and 60GHz wireless communication. The necessary image encoding, makes it challenging to maintain the stringent VR latency requirements. To achieve the required latency, our system employs a Parallel Rendering and Streaming mechanism to reduce the add-on streaming latency, by pipelining the rendering, encoding, transmission and decoding procedures. Furthermore, we introduce a Remote VSync Driven Rendering technique to minimize display latency. To evaluate the system, we implement an end-to-end remote rendering platform on commodity hardware over a 60Ghz wireless network. Results show that the system can support current 2160x1200 VR resolution at 90Hz with less than 16ms end-to-end latency, and 4K resolution with 20ms latency, while keeping a visually lossless image quality to the user.
</details>

 [📄 Paper](https://www.researchgate.net/profile/Luyang-Liu-3/publication/326240756_Cutting_the_Cord_Designing_a_High-quality_Untethered_VR_System_with_Low_Latency_Remote_Rendering/links/5b43e204aca2728a0d6898cc/Cutting-the-Cord-Designing-a-High-quality-Untethered-VR-System-with-Low-Latency-Remote-Rendering.pdf) 

<br>


 ### 5. Edge-Computing-Assisted Virtual Reality Computation Offloading: An Empirical Study
**Authors**: B. W. Nyamtiga, Airlangga Adi Hermawan, Y. F. Luckyarno, Tae-Wook Kim, Deok-Young Jung, Jin Sam Kwak, Ji-Hoon Yun
<details span>
<summary><b>Abstract</b></summary>
Offloading heavy virtual reality (VR) computational operations to a network edge computation entity is receiving increasing attention as a tool to wirelessly and energy efficiently provide low-end client devices with high-quality and immersive interactive VR services anytime and anywhere across the globe. In this work, we aim to provide an understanding of various characteristics of VR computation offloading through comprehensive experiments conducted using a prototype testbed for edge-assisted VR processing and streaming. First, we investigate the benefits of VR offloading in terms of computational load and power consumption reduction for a client device compared to standalone operation. Next, we measure VR traffic patterns, including frame size and data and packet rates with various settings, such as different resolution and encoding options. We also measure several performance metrics associated with the quality of experience, namely, frame rate, packet loss rate, and image quality, with various configuration settings. Then, we present latency measurement studies and investigate per-component latency with various settings. Furthermore, we report the rigorous experiments performed to study the impacts of latency and motion patterns on the black borders formed due to image reprojection and the overfilling technique used to eliminate these black borders.
</details>

 [📄 Paper](https://ieeexplore.ieee.org/ielx7/6287639/9668973/09881517.pdf) 

<br>

 ### 6. Edge Cloud-based Augmented Reality
**Authors**: Christoph Bachhuber, A. Martinez, R. Pries, Sebastian Eger, E. Steinbach
<details span>
<summary><b>Abstract</b></summary>
A convincing augmented reality (AR) experience requires vast computational resources, in particular for threedimensional mapping of the environment, pose estimation and high-quality rendering of virtual objects. Even today's most powerful mobile devices can not provide such computational resources and consequently limit the achievable quality of the augmentation. To tackle this issue, all computations necessary for AR can be offloaded to the Edge Cloud, such that the mobile device merely acts as a camera and display. This approach introduces additional processing steps, namely video communication, which we carefully evaluate with respect to their influence on the quality of experience and energy consumption. In the evaluation of our prototype, we show that with a Glassto-Glass delay of about 85 ms, our implementation is competitive against state-of-the-art solutions which run completely locally on a mobile device. Most notably, the additional steps required for offloading contribute little delay, which is often overcompensated by the faster computations in the Edge Cloud. A further benefit is that compared to performing all AR processing locally, offloading reduces the energy consumption in smartphones on average by 50 %. Moreover, the computational resources available for the AR application increase by a factor 10 to 100 through offloading. Finally, offloading enables high-quality AR applications even in low-end mobile devices.
</details>


<br>


 ### 7. Mobile VR on edge cloud: a latency-driven design
**Authors**: Shu Shi, Varun Gupta, Michael Hwang, R. Jana
<details span>
<summary><b>Abstract</b></summary>
In this paper we design and implement MEC-VR, a mobile VR system that uses a Mobile Edge Cloud (MEC) to deliver high quality VR content to today's mobile devices using 4G/LTE cellular networks. Our main contribution is in realizing a low latency control loop that streams VR scenes containing only the user's Field of View (FoV) and a latency-adaptive margin area around the FoV. This allows the clients to render locally at a high refresh rate to accommodate and compensate for the head movements before the next motion update arrives. Compared with prior approaches, our MEC-VR design requires no viewpoint prediction, supports dynamic and live VR content, and adapts to the real-world latency experienced in cellular networks between the MEC and mobile devices. We implement a prototype of MEC-VR and evaluate its performance on a MEC node connected to an LTE testbed. We demonstrate that MEC-VR can effectively stream live VR content up to 8K resolution over 4G/LTE networks and achieve more than 80% of bandwidth savings.
</details>

 [📄 Paper](https://www.researchgate.net/profile/Shu-Shi-3/publication/333862842_Mobile_VR_on_edge_cloud_a_latency-driven_design/links/5d51764a92851cd046b592df/Mobile-VR-on-edge-cloud-a-latency-driven-design.pdf) 

<br>


 ### 8. On the Minimization of Glass-to-Glass and Glass-to-Algorithm Delay in Video Communication
**Authors**: Christoph Bachhuber, E. Steinbach, Martin Freundl, M. Reisslein
<details span>
<summary><b>Abstract</b></summary>
Video cameras are increasingly used to provide realtime feedback in automatic control systems, such as autonomous driving and robotics systems. For such highly dynamic applications, the Glass-to-Glass (G2G) and Glass-to-Algorithm (G2A) latencies are critical. In this paper, we analyze the latencies in a point-to-point video transmission system and propose novel frame skipping and preemption approaches to reduce the G2G and G2A delays. We implement the proposed approaches in a prototype which shows significantly reduced G2G and G2A latencies as well as reduced transmission bitrate requirements compared with traditional video transmission schemes. In our low-delay video communication prototype, a VGA resolution video is transmitted with average G2G and G2A delays of 21.2 and 11.5 milliseconds with off-the-shelf hardware.
</details>

 [📄 Paper](https://faculty.engineering.asu.edu/mre/wp-content/uploads/sites/31/2020/04/DelVidComm.pdf) 

<br>


 ### 9. OpenUVR: an Open-Source System Framework for Untethered Virtual Reality Applications
**Authors**: Yunhua Deng, Yusen Li, Ronald Seet, Xueyan Tang, Wentong Cai
<details span>
<summary><b>Abstract</b></summary>
Advancements in heterogeneous computing technologies enable the significant potential of virtual reality (VR) applications. To offer the best user experience (UX), a system should adopt an untethered, wireless-network-based architecture to transfer VR content between the user and the content generator. However, modern wireless network technologies make implementing such an architecture challenging, as VR applications require superior video quality—with high resolution, high frame rates, and very low latency. This paper presents OpenUVR, an open-source framework that uses commodity hardware components to satisfy the demands of interactive, real-time VR applications. OpenUVR significantly improves UX through a redesign of the system stack and addresses the most time-sensitive issues associated with redundant memory copying in modern computing systems. OpenUVR presents a cross-layered VR datapath to avoid redundant data operations and computation among system components, OpenUVR customizes the network stack to eliminate unnecessary memory operations incurred by mismatching data formats in each layer, and OpenUVR uses feedback from mobile devices to remove memory buffers. Together, these modifications allow OpenUVR to reduce VR application delays to 14.32 ms, meeting the 20 ms minimum latency in avoiding motion sickness. As an open-source system that is fully compatible with commodity hardware, OpenUVR offers the research community an opportunity to develop, investigate, and optimize applications for untethered, high-performance VR architectures.
</details>

 [📄 Paper](https://par.nsf.gov/servlets/purl/10221134) 

<br>


 ### 10. Towards Fully Offloaded Cloud-based AR: Design, Implementation and Experience
**Authors**: R. Shea, Andy Sun, Silvery Fu, Jiangchuan Liu
<details span>
<summary><b>Abstract</b></summary>
Combining advanced sensors and powerful processing capabilities smart-phone based augmented reality (AR) is becoming increasingly prolific. e increase in prominence of these resource hungry AR applications poses significant challenges to energy constrained environments such as mobile-phones. To that end we present a platform for offloading AR applications to powerful cloud servers. We implement this system using a thin-client design and explore its performance using the real world application Pokemon Go as a case study. We show that with careful design a thin client is capable of offloading much of the AR processing to a cloud server, with the results being streamed back. Our initial experiments show substantial energy savings, low latency and excellent image quality even at relatively low bit-rates.
</details>

 [📄 Paper](https://drive.google.com/file/d/1_l5LFnHHr-f1HqBkRLt2lqpGS7QZZaxP/view) 

<br>


<br>

## Dataset

### 1. CGD: A Cloud Gaming Dataset with Gameplay Video and Network Recordings
**Authors**: Iva Slivar, K. Bačić, Irena Orsolic, Lea Skorin-Kapov, M. Sužnjević
<details span>
<summary><b>Abstract</b></summary>
With advances in network capabilities, the gaming industry is increasingly turning towards offering "gaming on demand" solutions, with cloud gaming services such as Sony PlayStation Now, Google Stadia, and NVIDIA GeForce NOW expanding their market offerings. Similar to adaptive video streaming services, cloud gaming services typically adapt the quality of game streams (e.g., bitrate, resolution, frame rate) in accordance with current network conditions. To select the most appropriate video encoding parameters given certain conditions, it is important to understand their impact on Quality of Experience (QoE). On the other hand, network operators are interested in understanding the relationships between parameters measurable in the network and cloud gaming QoE, to be able to invoke QoE-aware network management mechanisms. To encourage developments in these areas, comprehensive datasets are crucial, including both network and application layer data. This paper presents CGD, a dataset consisting of 600 game streaming sessions corresponding to 10 games of different genres being played and streamed using the following encoding parameters: bitrate (5, 10, 20 Mbps), resolution (720p, 1080p), and frame rate (30, 60 fps). For every combination repeated five times for each game, the dataset includes: 1) gameplay video recordings, 2) network traffic traces, 3) user input logs (mouse and keyboard), and 4) streaming performance logs.
</details>

 [📄 Paper](https://scholar.archive.org/work/r3decnunc5bole6x4g7epeow5y/access/wayback/https://dl.acm.org/doi/pdf/10.1145/3524273.3532898) 

<br>

### 2. GamingVideoSET: a dataset for gaming video streaming applications
**Authors**: Nabajeet Barman, Saman Zadtootaghaj, Steven Schmidt, M. Martini, S. Möller
<details span>
<summary><b>Abstract</b></summary>
This paper presents GamingVideoSET1, a dataset consisting of twenty-four uncompressed raw gaming videos of 30 seconds duration, 1080p resolution, and 30 fps for the research community working on gaming video quality assessment. Furthermore, the data set includes subjective quality assessment results for 90 video sequences obtained by encoding six different gaming videos using the H.264/MPEG-AVC codec standard in 15 different resolution-bitrate pairs (three resolution, five bitrates each). In addition to the reference videos, the dataset offers a total of 576 distorted videos in MP4 format, obtained by encoding the videos in 24 different resolution-bitrate pairs, and their objective quality assessment results (average and per-frame) using three video quality assessment metrics.
</details>

 [📄 Paper](https://www.researchgate.net/profile/Nabajeet-Barman-2/publication/325285210_GamingVideoSET_A_Dataset_for_Gaming_Video_Streaming_Applications/links/605f34fc458515e83476bee8/GamingVideoSET-A-Dataset-for-Gaming-Video-Streaming-Applications.pdf) | [💻 Code ](https://github.com/NabajeetBarman/GamingHDRVideoSET)

<br>

### 3. User generated HDR gaming video streaming : dataset, codec comparison and challenges
**Authors**: Nabajeet Barman, M. Martini
<details span>
<summary><b>Abstract</b></summary>
Gaming video streaming services have grown tremendously in the past few years, with higher resolutions, higher frame rates and HDR gaming videos getting increasingly adopted among the gaming community. Since gaming content as such is different from non-gaming content, it is imperative to evaluate the performance of the existing encoders to help understand the bandwidth requirements of such services, as well as further improve the compression efficiency of such encoders. Towards this end, we present in this paper GamingHDRVideoSET1, a dataset consisting of eighteen 10-bit UHD-HDR gaming videos and encoded video sequences using four different codecs, together with their objective evaluation results. Additionally, the paper discusses the codec compression efficiency of most widely used practical encoders, i.e., x264 (H.264/AVC), x265 (H.265/HEVC) and libvpx (VP9), as well the recently proposed encoder libaom (AV1), on 10-bit, UHD-HDR content gaming content. Our results show that the latest compression standard AV1 results in the best compression efficiency, followed by HEVC, H.264, and VP9.
</details>

 [📄 Paper](https://eprints.kingston.ac.uk/id/eprint/49080/6/Barman-N-49080-1-AAM.pdf) | [💻 Code ](https://github.com/NabajeetBarman/GamingHDRVideoSET)

<br>

### 4. Video Coding Tool Analysis and Dataset for Gaming Content
**Authors**: Xin Zhao, Shankai Liu, Xiang Li, Guichun Li, Xiaozhong Xu
<details span>
<summary><b>Abstract</b></summary>
The gaming market has kept growing significantly in recent years. Driven by multiple technology advances, such as cloud computing and video technologies, new gaming applications, e.g. AR, VR and cloud gaming, are becoming more and more practical and popular. Among different types of gaming, the emergence of cloud gaming is driving the market with enhanced gamer experience as well as new challenges to the services. One of the key technological challenges of gaming applications is the video coding, which is the foundation of several popular gaming applications, including cloud gaming and game live streaming. Comparing to the typical camera captured content and screen content, gaming content presents unique features that directly lead to different preferences on the selection of coding tool sets. To better understand the behaviors of known video coding tools and provide test materials for research and development on future coding tools that benefits more on gaming content, in this paper, a dataset consists of a set of gaming video is proposed together with analysis of the performances of existing coding tools on these materials. It is observed that, several known coding tools are exceptionally beneficial for gaming content and the rational is analyzed in this paper.
</details>

<br>

## Edge 5G

### 1. A Comprehensive Survey on Mobile Edge Computing: Challenges, Tools, Applications
**Authors**: Fatema Vhora, Jay Gandhi
<details span>
<summary><b>Abstract</b></summary>
Mobile edge computing (MEC) is an emerging standard where cloud computing services like storage and computing, provide to the edge of networks. MEC has the potential of executing computing-intensive applications such as augmented and virtual reality. It is an essential component in the internet of things (IoT) and 5G architecture that provides a noticeable reduction in latency and energy consumption of mobile devices. This paper covers a comprehensive survey about the MEC concept including MEC Analogue. It presents a different edge paradigm like Fog computing, cloudlet, MEC, along with its architecture. The diverse challenges with its related work are covers during the survey. Simulation tools and challenges for real time implementations are explained. Finally, different MEC Scenarios and applications are discussed.
</details>

 [📄 Paper](https://www.researchgate.net/profile/Fatema-Vhora/publication/340895452_A_Comprehensive_Survey_on_Mobile_Edge_Computing_Challenges_Tools_Applications/links/5ee4818c299bf1faac526a87/A-Comprehensive-Survey-on-Mobile-Edge-Computing-Challenges-Tools-Applications.pdf)

<br>


### 2. Computation Offloading Toward Edge Computing
**Authors**: Li Lin, Xiaofei Liao, Hai Jin, Peng Li
<details span>
<summary><b>Abstract</b></summary>
We are living in a world where massive end devices perform computing everywhere and everyday. However, these devices are constrained by the battery and computational resources. With the increasing number of intelligent applications (e.g., augmented reality and face recognition) that require much more computational power, they shift to perform computation offloading to the cloud, known as mobile cloud computing (MCC). Unfortunately, the cloud is usually far away from end devices, leading to a high latency as well as the bad quality of experience (QoE) for latency-sensitive applications. In this context, the emergence of edge computing is no coincidence. Edge computing extends the cloud to the edge of the network, close to end users, bringing ultra-low latency and high bandwidth. Consequently, there is a trend of computation offloading toward edge computing. In this paper, we provide a comprehensive perspective on this trend. First, we give an insight into the architecture refactoring in edge computing. Based on that insight, this paper reviews the state-of-the-art research on computation offloading in terms of application partitioning, task allocation, resource management, and distributed execution, with highlighting features for edge computing. Then, we illustrate some disruptive application scenarios that we envision as critical drivers for the flourish of edge computing, such as real-time video analytics, smart “things” (e.g., smart city and smart home), vehicle applications, and cloud gaming. Finally, we discuss the opportunities and future research directions.
</details>


<br>


### 3. From cloud to edge: a first look at public edge platforms
**Authors**: Mengwei Xu, Zhe Fu, Xiao Ma, Li Zhang, Yanan Li, Feng Qian, Shangguang Wang, Ke Li, Jingyu Yang, Xuanzhe Liu
<details span>
<summary><b>Abstract</b></summary>
Public edge platforms have drawn increasing attention from both academia and industry. In this study, we perform a first-of-its-kind measurement study on a leading public edge platform that has been densely deployed in China. Based on this measurement, we quantitatively answer two critical yetunexplored questions. First, from end users' perspective, what is the performance of commodity edge platforms compared to cloud, in terms of the end-to-end network delay, throughput, and the application QoE. Second, from the edge service provider's perspective, how are the edge workloads different from cloud, in terms of their VM subscription, monetary cost, and resource usage. Our study quantitatively reveals the status quo of today's public edge platforms, and provides crucial insights towards developing and operating future edge services.
</details>

 [📄 Paper](https://feng-qian.github.io/paper/edge_imc21.pdf) | [💻 Code ](https://feng-qian.github.io/index.html)

<br>

### 4. Improving Cloud Gaming Experience through Mobile Edge Computing
**Authors**: Xu Zhang, Hao Chen, Yangchao Zhao, Zhan Ma, Yiling Xu, Haojun Huang, H. Yin, Dapeng Oliver Wu
<details span>
<summary><b>Abstract</b></summary>
With the development of 4G/5G technology and smart devices, more and more users begin to play games via their mobile devices. As a promising way to enable users to play any games, cloud gaming is proposed to stream game scene rendered remotely in the cloud with the format of video. However, it faces major challenges in terms of long delay and high network bandwidth. To this end, a novel framework named EdgeGame is proposed to improve the cloud gaming experience by leveraging resources in the edge. Compared to existing cloud gaming systems, EdgeGame offloads the computation-intensive rendering to the network edge instead, which can reduce network delay and bandwidth consumption greatly. Moreover, EdgeGame introduces deep reinforcement learning in the edge to adjust the video bitrates adaptively to accommodate the network dynamics. Finally, we implemented a prototype system and compared it with an existing cloud gaming system. The experiments show that EdgeGame can reduce the average network delay by 50 percent and improve user's QoE by 20 percent.
</details>

 [📄 Paper](https://www.researchgate.net/profile/Haojun-Huang-2/publication/344771771_Improving_Cloud_Gaming_Experience_through_Mobile_Edge_Computing/links/643e961f39aa471a524890e8/Improving-Cloud-Gaming-Experience-through-Mobile-Edge-Computing.pdf) 

<br>

## Latency

### 1. A Measurement Study on Achieving Imperceptible Latency in Mobile Cloud Gaming
**Authors**: Teemu Kämäräinen, M. Siekkinen, Antti Ylä-Jääski, Wenxiao Zhang, P. Hui
<details span>
<summary><b>Abstract</b></summary>
Cloud gaming is a relatively new paradigm in which the game is rendered in the cloud and is streamed to an end-user device through a thin client. Latency is a key challenge for cloud gaming. In order to optimize the end-to-end latency, it is first necessary to understand how the end-to-end latency builds up from the mobile device to the cloud gaming server. In this paper we dissect the delays occurring in the mobile device and measure access delays in various networks and network conditions. We also perform a Europe-wide latency measurement study to find the optimal server locations and see how the number of server locations affects the network delay. The results are compared to limits found for perceivable delays in recent human-computer interaction studies. We show that the limits can be achieved only with the latest mobile devices with specific control methods. In addition, we study the expected latency reduction by near future technological development and show that its potential impact is bigger on the end-to-end latency than that of replication of the service and server placement optimization.
</details>

 [📄 Paper](https://pdfs.semanticscholar.org/b43f/9c0a6e424c2730265a2f42bd66c441092c0e.pdf) 


### 2. A System for Precise End-to-End Delay Measurements in Video Communication.
**Authors**: Christoph Bachhuber, E. Steinbach
<details span>
<summary><b>Abstract</b></summary>
Ultra low delay video transmission is becoming increasingly important. Video-based applications with ultra low delay requirements range from teleoperation scenarios such as controlling drones or telesurgery to autonomous control of dynamic processes using computer vision algorithms applied on real-time video. To evaluate the performance of the video transmission chain in such systems, it is important to be able to precisely measure the glass-to-glass (G2G) delay of the transmitted video. In this paper1, we present a lowcomplexity system that takes a series of pairwise independent measurements of G2G delay and derives performance metrics such as mean delay or minimum delay etc. from the data. The precision is in the sub-millisecond range, mainly limited by the sampling rate of the measurement system. In our implementation, we achieve a G2G measurement precision of 0.5 milliseconds with a sampling rate of 2kHz.
</details>

 [📄 Paper](https://arxiv.org/pdf/1510.01134) 

<br>

### 3. Delay-Sensitive Video Computing in the Cloud: A Survey
**Authors**: M. Abdallah, C. Griwodz, Kuan-Ta Chen, G. Simon, Pin-Chun Wang, Cheng-Hsin Hsu
<details span>
<summary><b>Abstract</b></summary>
While cloud servers provide a tremendous amount of resources for networked video applications, most successful stories of cloud-assisted video applications are presentational video services, such as YouTube and NetFlix. This article surveys the recent advances on delay-sensitive video computations in the cloud, which are crucial to cloud-assisted conversational video services, such as cloud gaming, Virtual Reality (VR), Augmented Reality (AR), and telepresence. Supporting conversational video services with cloud resources is challenging because most cloud servers are far away from the end users while these services incur the following stringent requirements: high bandwidth, short delay, and high heterogeneity. In this article, we cover the literature with a top-down approach: from applications and experience, to architecture and management, and to optimization in and outside of the cloud. We also point out major open challenges, hoping to stimulate more research activities in this emerging and exciting direction.
</details>

 [📄 Paper](https://people.computing.clemson.edu/~jmarty/projects/lowLatencyNetworking/papers/RecentInternetMeasurementResearch/DelaySensitiveVideoComputingIntheCloud.pdf) 

<br>



### 4. Measuring the latency of cloud gaming systems
**Authors**: Kuan-Ta Chen, Yu-Chun Chang, P. Tseng, Chun-Ying Huang, C. Lei
<details span>
<summary><b>Abstract</b></summary>
Cloud gaming, i.e., real-time game playing via thin clients, relieves players from the need to constantly upgrade their computers and deal with compatibility issues when playing games. As a result, cloud gaming is generating a great deal of interest among entrepreneurs and the public. However, given the large design space, it is not yet known which platforms deliver the best quality of service and which design elements constitute a good cloud gaming system. This study is motivated by the question: How good is the real-timeliness of current cloud gaming systems? To address the question, we analyze the response latency of two cloud gaming platforms, namely, OnLive and StreamMyGame. Our results show that the streaming latency of OnLive is reasonable for real-time cloud gaming, while that of StreamMyGame is almost twice the former when the StreamMyGame server is provisioned using an Intel Core i7-920 PC. We believe that our measurement approach can be generally applied to PC-based cloud gaming platforms, and that it will further the understanding of such systems and lead to improvements.
</details>

 [📄 Paper](https://scholar.archive.org/work/26zari3d2vc77mcpiykzkvdxxy/access/wayback/http://mmnet.iis.sinica.edu.tw/pub/chen11_cloudgaming.pdf) 

<br>


### 5. The brewing storm in cloud gaming: a measurement study on cloud to end-user latency
**Authors**: Sharon Choy, B. Wong, G. Simon, C. Rosenberg
<details span>
<summary><b>Abstract</b></summary>
Cloud computing has been a revolutionary force in changing the way organizations deploy web applications and services. However, many of cloud computing's core design tenets, such as consolidating resources into a small number of datacenters and fine-grain partitioning of general purpose computing resources, conflict with an emerging class of multimedia applications that is highly latency sensitive and requires specialized hardware, such as graphic processing units (GPUs) and fast memory. In this paper, we look closely at one such application, namely, on-demand gaming (also known as cloud gaming), that has the potential to radically change the multi-billion dollar video game industry. We demonstrate through a large-scale measurement study that the current cloud computing infrastructure is unable to meet the strict latency requirements necessary for acceptable game play for many end-users, thus limiting the number of potential users for an on-demand gaming service. We further investigate the impact of augmenting the current cloud infrastructure with servers located near the end-users, such as those found in content distribution networks, and show that the user coverage significantly increases even with the addition of only a small number of servers.
</details>

 [📄 Paper](https://ece.uwaterloo.ca/~cath/edgecloud.pdf) 

<br>


### 6. The Effects of Latency in Commercial Cloud Video Gaming Services
**Authors**: V Courtemanche, A Desveaux 
<details span>
<summary><b>Abstract</b></summary>
Video games are typically played on a device such as a computer, console, or phone,with most of the computation on the local hardware. Cloud gaming services which take overmost computation have been rising in popularity as a potentially viable alternative to traditionalgaming. However, cloud gaming services are more susceptible to latency, since player inputsare sent to cloud servers, and video is then streamed back to the player's client. Our projectevaluated two recently released cloud gaming services (Blade Shadow and Google Stadia) todetermine how they were affected by increased latency and packet loss. We performed a userstudy with different added latency values to test player performance and quality of experiencefor each service. We then performed network experiments analyzing the effects of addedlatency and packet loss on bitrates. Analysis of 37 users shows that user performance andquality of experience decreased with higher added latency for both services. Shadow usedsignificantly more bandwidth than Stadia but had better graphics quality.
</details>

 [📄 Paper](http://web.cs.wpi.edu/~claypool/iqp/cloudgame-19/report.pdf)

<br>

<br>

## QoE

### 1. A game attention model for efficient bit rate allocation in cloud gaming
**Authors**:H. Ahmadi, Saman Zad Tootaghaj, M. Hashemi, S. Shirmohammadi
<details span>
<summary><b>Abstract</b></summary>
The widespread availability of broadband internet access and the growth in server-based processing have provided an opportunity to run games away from the player into the cloud and offer a new promising service known as cloud gaming. The concept of cloud gaming is to render a game in the cloud and stream the resulting game scenes to the player as a video sequence over a broadband connection. To meet the stringent network bandwidth requirements of cloud gaming and support more players, efficient bit rate reduction techniques are needed. In this paper, we introduce the concept of game attention model (GAM), which is basically a game context-based visual attention model, as a means for reducing the bit rate of the streaming video more efficiently. GAM estimates the importance of each macro-block in a game frame from the player's perspective and allows encoding the less important macro-blocks with lower bit rate. We have evaluated nine game video sequences, covering a wide range of game genre and a spectrum of scene content in terms of details, motion and brightness. Our subjective assessment shows that by integrating this model into the cloud gaming framework, it is possible to decrease the required bit rate by nearly 25 % on average, while maintaining a relatively high user quality of experience. This clearly enables players with limited communication resources to benefit from cloud gaming with acceptable quality.
</details>

 [📄 Paper](http://www.eiti.uottawa.ca/~shervin/pubs/GameStreaming-Springer-MMSJ.pdf)

<br>

### 2. An Evaluation of QoE in Cloud Gaming Based on Subjective Tests
**Authors**:M. Jarschel, D. Schlosser, Sven Scheuring, T. Hossfeld
<details span>
<summary><b>Abstract</b></summary>
Cloud Gaming is a new kind of service, which combines the successful concepts of Cloud Computing and Online Gaming. It provides the entire game experience to the users remotely from a data center. The player is no longer dependent on a specific type or quality of gaming hardware, but is able to use common devices. The end device only needs a broadband internet connection and the ability to display High Definition (HD) video. While this may reduce hardware costs for users and increase the revenue for developers by leaving out the retail chain, it also raises new challenges for service quality in terms of bandwidth and latency for the underlying network. In this paper we present the results of a subjective user study we conducted into the user-perceived quality of experience (QoE) in Cloud Gaming. We design a measurement environment, that emulates this new type of service, define tests for users to assess the QoE, derive Key Influence Factors (KFI) and influences of content and perception from our results.
</details>

 [📄 Paper](https://www.researchgate.net/profile/Tobias-Hossfeld/publication/215752557_An_Evaluation_of_QoE_in_Cloud_Gaming_Based_on_Subjective_Tests/links/0deec51c8aaf49b67a000000/An-Evaluation-of-QoE-in-Cloud-Gaming-Based-on-Subjective-Tests.pdf)

<br>

### 3. Analysis and QoE evaluation of cloud gaming service adaptation under different network conditions: The case of NVIDIA GeForce NOW
**Authors**:M. Suznjevic, Iva Slivar, L. Skorin-Kapov
<details span>
<summary><b>Abstract</b></summary>
Cloud gaming represents a highly interactive service whereby game logic is rendered in the cloud and streamed as a video to end devices. While benefits include the ability to stream high-quality graphics games to practically any end user device, drawbacks include high bandwidth requirements and very low latency. Consequently, a challenge faced by cloud gaming service providers is the design of algorithms for adapting video streaming parameters to meet the end user system and network resource constraints. In this paper, we conduct an analysis of the commercial NVIDIA GeForce NOW game streaming platform adaptation mechanisms in light of variable network conditions. We further conduct an empirical user study involving the GeForce NOW platform to assess player Quality of Experience when such adaptation mechanisms are employed. The results provide insight into limitations of the currently deployed mechanisms, as well as aim to provide input for the proposal of designing future video encoding adaptation strategies.
</details>

 [📄 Paper](http://www.fer.unizg.hr/_news/66573/QoMEX_2016.pdf)

<br>

### 4. Delay Sensitivity Classification of Cloud Gaming Content
**Authors**:S. Sabet, Steven Schmidt, Saman Zadtootaghaj, C. Griwodz, Sebastian Möller
<details span>
<summary><b>Abstract</b></summary>
Cloud Gaming is an emerging service that catches growing interestin the research community as well as industry. Cloud Gamingrequire a highly reliable and low latency network to achieve asatisfying Quality of Experience (QoE) for its users. Using a cloudgaming service with high latency would harm the interaction of theuser with the game, leading to a decrease in playing performanceand, thus players frustrations. However, the negative effect of delayon gaming QoE depends strongly on the game content. At a certainlevel of delay, a slow-paced card game is typically not as delaysensitive as a shooting game. For optimal resource allocation andquality estimation, it is highly important for cloud providers, gamedevelopers, and network planners to consider the impact of thegame content. This paper contributes to a better understanding ofthe delay impact on QoE for cloud gaming applications byidentifying game characteristics influencing the delay perception ofthe users. In addition, an expert evaluation methodology to quantifythese characteristics as well as a delay sensitivity classificationbased on a decision tree are presented. The results indicated anexcellent level of agreement, which demonstrates the reliability ofthe proposed method. Additionally, the decision tree reached anaccuracy of 90% on determining the delay sensitivity classes whichwere derived from a large dataset of subjective input quality ratingsduring a series of experiments.
</details>

 [📄 Paper](https://arxiv.org/abs/2004.05609)

<br>

### 5. Game Categorization for Deriving QoE-Driven Video Encoding Configuration Strategies for Cloud Gaming
**Authors**:Iva Slivar, M. Sužnjević, Lea Skorin-Kapov
<details span>
<summary><b>Abstract</b></summary>
Cloud gaming has been recognized as a promising shift in the online game industry, with the aim of implementing the "on demand" service concept that has achieved market success in other areas of digital entertainment such as movies and TV shows. The concepts of cloud computing are leveraged to render the game scene as a video stream that is then delivered to players in real-time. The main advantage of this approach is the capability of delivering high-quality graphics games to any type of end user device; however, at the cost of high bandwidth consumption and strict latency requirements. A key challenge faced by cloud game providers lies in configuring the video encoding parameters so as to maximize player Quality of Experience (QoE) while meeting bandwidth availability constraints. In this article, we tackle one aspect of this problem by addressing the following research question: Is it possible to improve service adaptation based on information about the characteristics of the game being streamed? To answer this question, two main challenges need to be addressed: the need for different QoE-driven video encoding (re-)configuration strategies for different categories of games, and how to determine a relevant game categorization to be used for assigning appropriate configuration strategies. We investigate these problems by conducting two subjective laboratory studies with a total of 80 players and three different games. Results indicate that different strategies should likely be applied for different types of games, and show that existing game classifications are not necessarily suitable for differentiating game types in this context. We thus further analyze objective video metrics of collected game play video traces as well as player actions per minute and use this as input data for clustering of games into two clusters. Subjective results verify that different video encoding configuration strategies may be applied to games belonging to different clusters.
</details>

 [📄 Paper](https://tel.fer.hr/images/50020394/ACM%20TOMM%20Game%20Categorization%20QoE-Driven%20Video%20Encoding%20Configuration%20Cloud%20Gaming_PREPRINT.pdf)

<br>

### 6. Latency impact on Quality of Experience in a virtual reality simulator for remote control of machines
**Authors**:
<details span>
<summary><b>Abstract</b></summary>
In this article, we have investigated a VR simulator of a forestry crane used for loading logs onto a truck. We have mainly studied the Quality of Experience (QoE) aspects that may be relevant for task completion, and whether there are any discomfort related symptoms experienced during the task execution. QoE experiments were designed to capture the general subjective experience of using the simulator, and to study task performance. The focus was to study the effects of latency on the subjective experience, with regards to delays in the crane control interface. Subjective studies were performed with controlled delays added to the display update and hand controller (joystick) signals. The added delays ranged from 0 to 30 ms for the display update, and from 0 to 800 ms for the hand controller. We found a strong effect on latency in the display update and a significant negative effect for 800 ms added delay on latency in the hand controller (in total approx. 880 ms latency including the system delay). The Simulator Sickness Questionnaire (SSQ) gave significantly higher scores after the experiment compared to before the experiment, but a majority of the participants reported experiencing only minor symptoms. Some test subjects ceased the test before finishing due to their symptoms, particularly due to the added latency in the display update.
</details>

 [📄 Paper](https://www.academia.edu/download/64667759/RMVis_1347_Latency_impact_on_QoE_1-s2.0-S0923596520301648-main.pdf)

<br>

### 7. Modeling Gaming QoE: Towards the Impact of Frame Rate and Bit Rate on Cloud Gaming
**Authors**:Saman Zadtootaghaj, Steven Schmidt, Sebastian Möller
<details span>
<summary><b>Abstract</b></summary>
Recent advances of streaming services and the upcoming new generation of mobile networks, 5G, offering low end-to-end delay as well as high bandwidths, promise a bright future for cloud gaming applications. Cloud gaming, in the contrary to traditional gaming services, suffers not only from system factors on the client, but is also affected significantly by the network, server specification and encoding parameters. In this paper, we present the results of a subjective experiment aiming to investigate the impact of two influencing factors, frame rate and bit rate, on the gaming Quality of Experience. The results reveal that a trade-off between an acceptable video quality and interaction quality exists. In case of very low bit rates, lowering the frame rate can improve the video quality while at some point, jerkiness becomes visible which affects the video quality negatively and the control over the game will be strongly reduced. Furthermore, even though in the gaming community a frame rate of 60 fps is desired, no significant difference for quality ratings, as well as performance ratings, was found between 60 fps and 25 fps. Therefore, it would be highly valuable for service providers to find an ideal strategy for this issue. In addition, we investigate the impact of video encoding on gaming experience dimensions. Finally, a first attempt to model the impact of two influencing factors on overall quality will be presented.
</details>

 [📄 Paper](https://ieeexplore.ieee.org/document/8463416)

<br>

### 8. Perceived order in different sense modalities.
**Authors**:I. Hirsh, C. Sherrick
<details span>
<summary><b>Abstract</b></summary>

</details>

 [📄 Paper]()

<br>

### 9. Quality of experience (QoE) in cloud gaming models: A review
**Authors**:Asif Ali Laghari, Hui He, K. A. Memon, Rashid Ali Laghari, I. A. Halepoto, Asiya Khan
<details span>
<summary><b>Abstract</b></summary>
Cloud gaming is a new way of online gaming, which renders the game data on the cloud side instead of the end user's system and is forwarded via a high-speed network. In cloud gaming; game software and emulators run on the high-speed server of cloud and services available for users on the commercial and free basis. Users can use rendered data of game from the cloud using thin heterogeneous devices via the Internet to play the game anytime and anywhere. The popularity of cloud gaming has increased since the late 2000s which attract the industry and academia. Quality of experience (QoE) domain has been added in cloud gaming models to assess user satisfaction, enjoyment, and needs during online gaming. In this research paper; we survey and analyze the previous cloud gaming models and models and offer aspects of future development; which will help to give the quality of service (QoS) according to service level agreement (SLA) and increase user satisfaction level for cloud gaming, hence, improving the overall QoE.
</details>

 [📄 Paper](https://pearl.plymouth.ac.uk/bitstream/handle/10026.1/14894/cloud%20Gaming%20Review.pdf?sequence=1)

<br>


### 10. Subjective quality assessment for cloud gaming
**Authors**:Abdul Wahab, Nafi Ahmad, M. Martini, J. Schormans
<details span>
<summary><b>Abstract</b></summary>
Using subjective testing, we study the effect of the network parameters, delay and packet loss ratio, on the QoE of cloud gaming. We studied three different games, selected based on genre, popularity, content complexity and pace, and tested them in a controlled network environment, using a novel emulator to create realistic lognormal delay distributions instead of relying on a static mean delay, as used previously; we also used Parsec as a good representative of the state of the art. We captured user ratings on an ordinal Absolute Category Rating scale for three quality dimensions: Video QoE, Game-Playability QoE, and Overall QoE. We show that Mean Opinion Scores (MOS) for the game with the highest levels of content complexity and pace are most severely affected by network impairments. We also show that the QoE of interactive cloud applications rely more on the game playability than the video quality of the game. Unlike earlier studies, the differences in MOS are validated using the distributions of the underlying dimensions. A Wilcoxon Signed-Rank test showed that the distributions of Video QoE and Game Playability QoE are not significantly differen.
</details>

 [📄 Paper](https://pdfs.semanticscholar.org/b882/84bfa3176671f7cebcc7c71225d2e2c1a24a.pdf)

<br>

## QoS

### 1. A First Look at the Network Turbulence for Google Stadia Cloud-based Game Streaming
**Authors**:
<details span>
<summary><b>Abstract</b></summary>

</details>

 [📄 Paper]()

<br>

### 2. A network analysis on cloud gaming: Stadia, GeForce Now and PSNow
**Authors**:
<details span>
<summary><b>Abstract</b></summary>

</details>

 [📄 Paper]()

<br>

### 3. A survey on quality of service in cloud computing
**Authors**:
<details span>
<summary><b>Abstract</b></summary>

</details>

 [📄 Paper]()

<br>

### 4. An Analysis of Cloud Gaming Platforms Behavior under Different Network Constraints
**Authors**:
<details span>
<summary><b>Abstract</b></summary>

</details>

 [📄 Paper]()

<br>

### 5. Cloud-gaming: Analysis of Google Stadia traffic.
**Authors**:
<details span>
<summary><b>Abstract</b></summary>

</details>

 [📄 Paper]()

<br>

### 6. Demystifying the Largest Live Game Streaming Platform via Black-Box Measurement
**Authors**:
<details span>
<summary><b>Abstract</b></summary>

</details>

 [📄 Paper]()

<br>

### 7. Measuring Key Quality Indicators in Cloud Gaming: Framework and Assessment Over Wireless Networks
**Authors**:
<details span>
<summary><b>Abstract</b></summary>

</details>

 [📄 Paper]()

<br>

### 8. On the Quality of Service of Cloud Gaming Systems
**Authors**:Kuan-Ta Chen, Yu-Chun Chang, Hwai-Jung Hsu, De-Yu Chen, Chun-Ying Huang, Cheng-Hsin Hsu
<details span>
<summary><b>Abstract</b></summary>
Cloud gaming, i.e., real-time game playing via thin clients, relieves users from being forced to upgrade their computers and resolve the incompatibility issues between games and computers. As a result, cloud gaming is generating a great deal of interests among entrepreneurs, venture capitalists, general publics, and researchers. However, given the large design space, it is not yet known which cloud gaming system delivers the best user-perceived Quality of Service (QoS) and what design elements constitute a good cloud gaming system.This study is motivated by the question: How good is the QoS of current cloud gaming systems? Answering the question is challenging because most cloud gaming systems are proprietary and closed, and thus their internal mechanisms are not accessible for the research community. In this paper, we propose a suite of measurement techniques to evaluate the QoS of cloud gaming systems and prove the effectiveness of our schemes using a case study comprising two well-known cloud gaming systems: OnLive and StreamMyGame. Our results show that OnLive performs better, because it provides adaptable frame rates, better graphic quality, and shorter server processing delays, while consuming less network bandwidth. Our measurement techniques are general and can be applied to any cloud gaming systems, so that researchers, users, and service providers may systematically quantify the QoS of these systems. To the best of our knowledge, the proposed suite of measurement techniques have never been presented in the literature.
</details>

 [📄 Paper](https://homepage.iis.sinica.edu.tw/~swc/pub/qos_cloud_gaming_systems.html)

<br>

### 9. Performance Measurements on a Cloud VR Gaming Platform
**Authors**:
<details span>
<summary><b>Abstract</b></summary>

</details>

 [📄 Paper]()

<br>

### 10. Playing High-End Video Games in the Cloud: A Measurement Study
**Authors**:
<details span>
<summary><b>Abstract</b></summary>

</details>

 [📄 Paper]()

<br>

### 11. The Effects of Latency, Bandwidth, and Packet Loss on Cloud-Based Gaming Services
**Authors**:
<details span>
<summary><b>Abstract</b></summary>

</details>

 [📄 Paper]()

<br>

## Streaming

<br>

<br>

## Survey

<br>

<br>

## Virtulized

<br>

<br>

## Open Source Implementations

<br>

## Credits

- Thanks to 
