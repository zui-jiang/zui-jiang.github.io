---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a Master's student in the University Chinese Academy of Sciences, under the supervision of Professor [Ben He](https://people.ucas.ac.cn/~benhe?language=en). 

My research interests include:
 - Scalable Oversight
 - LLM Safety
 - Multi-modal LLM 
 - Mechanistic interpretability


---
# Publications
## 2025
- **Auto-RT: Automatic Jailbreak Strategy Exploration for Red-Teaming Large Language Models**
  **Yanjiang Liu**, Shuhen Zhou, Yaojie Lu, Huijia Zhu, Weiqiang Wang, Hongyu Lin, Ben He, Xianpei Han, Le Sun
  *arXiv preprint*  
  [[Paper]](https://arxiv.org/pdf/2501.01830) [[Code]](https://github.com/icip-cas/Auto-RT)

- **SAISA: Towards Multimodal Large Language Models with Both Training and Inference Efficiency**
  Qianhao Yuan\*, **Yanjiang Liu\***, Yaojie Lu, Hongyu Lin, Ben He, Xianpei Han, Le Sun
  *arXiv preprint*  
   [[Code]](https://github.com/icip-cas/SAISA)

- **Expanding the Boundaries of Vision Prior Knowledge in Multi-modal Large Language Models**
  Qiao Liang\*, **Yanjiang Liu\***, Ben He, Yaojie Lu, Hongyu Lin, Xianpei Han, Le Sun, Yingfei Sun
  *arXiv preprint*  

## 2024
- **Search, Verify and Feedback: Towards Next Generation Post-training Paradigm of Foundation Models via Verifier Engineering**  
  Xinyan Guan, **Yanjiang Liu**, Xinyu Lu, Boxi Cao, Ben He, Xianpei Han, Le Sun, Jie Lou, Bowen Yu, Yaojie Lu, Hongyu Lin  
  *arXiv preprint arXiv:2411.11504*  
  [[Paper]](https://arxiv.org/abs/2411.11504) [[Github]](https://github.com/icip-cas/Verifier-Engineering/tree/main)

- **Mitigating Large Language Model Hallucinations via Autonomous Knowledge Graph-based Retrofitting**  
  Xinyan Guan, **Yanjiang Liu**, Hongyu Lin, Yaojie Lu, Ben He, Xianpei Han, Le Sun  
  *AAAI Conference on Artificial Intelligence (AAAI 2024)*  
  [[Paper]](https://arxiv.org/abs/2311.13314)

- **XMC-Agent: Dynamic Navigation over Scalable Hierarchical Index for Incremental Extreme Multi-label Classification**  
  **Yanjiang Liu**, **Tianyun Zhong**, **Yaojie Lu**, **Hongyu Lin**, **Ben He**, **Shuheng Zhou**, **Huijia Zhu**, **Weiqiang Wang**, **Zhongyi Liu**, **Xianpei Han**, **Le Sun** 
  *Annual Meeting of the Association for Computational Linguistics (ACL 2024 findings)*  
  [[Paper]](https://aclanthology.org/2024.findings-acl.336.pdf) [[Code]](https://github.com/zui-jiang/XMC-AGENT)


<script>
  // 获取访客的IP地址并通过API获取地理位置信息
  fetch('https://ipinfo.io?token=your_token')
    .then(response => response.json())
    .then(data => {
      const [lat, lon] = data.loc.split(',');
      
      // 初始化 Google Map
      const map = new google.maps.Map(document.getElementById('map'), {
        center: { lat: parseFloat(lat), lng: parseFloat(lon) },
        zoom: 10
      });
      
      // 添加标记
      new google.maps.Marker({
        position: { lat: parseFloat(lat), lng: parseFloat(lon) },
        map: map
      });
    });
</script>
<!-- Google Maps API -->
<script src="https://maps.googleapis.com/maps/api/js?key=your_google_maps_api_key&callback=initMap" async defer></script>

<div id="map" style="height: 400px;"></div>