# AIDM-7460

## **Individual Project**
Future of Auto News or the Coming Flood of Disinformation? A Practical Inspection and Exploration of ChatGPT’s Auto-generated Chinese News

###  **Content Introduction**
```
│   main.ipynb
                \\ Main notebook for all ChatGPT contents generation and visualization part.
│   model_train.ipynb
                \\ Fake News Detection Model building and practicle detection part.
│ 
|||||||||||||||||||||||||| Model Related
│   grid_search.py
│   layers.py
│   main.py
├───data
│   ├───ch
│   │       test.pkl
│   │       train.pkl
│   │       val.pkl
│   │       
│   └───en
│           test.pkl
│           train.pkl
│           val.pkl
│||||||||||||||||||||||||| Model Related


├───dataset
│       codebook.txt
|               \\ Codebook for Chinese Words Splitting.
│       NewsData.csv
|               \\ Input contents for ChatGPT generation.
│       news_generated_data_final.csv
|               \\ Dataset for auto-generated news and labeling results.
│       
├───external
│       Alibaba-PuHuiTi-Medium.ttf
|               \\ Wordcloud generation needed.
│       
├───images
│       All Results.png
│       Average Faults Count by Fact.png
│       Boxplot of Faults Count by Fact.png
│       Commentary Results by Media.png
│       Commentary Results.png
│       Correctness by Category.png
│       Correctness by Commentary.png
│       Detailed Counts of Correctness by Facts.png
│       FScore vs Epoch.png
│       Predicted Correctness Results.png
│       Predicted Correctness vs Category.png
│       Predicted Correctness vs correctness.png
│       Predicted Results.png
│       Wordcloud.png


│||||||||||||||||||||||||| Model Related      
├───logs
│   ├───json
│   │       mdfend.json
│   │       
│   └───param
│           bert_oneloss_param.txt
│           m3fend_oneloss_param.txt
│           mdfend_oneloss_param.txt         
├───models
│       mdfend.py     
├───param_model
└───utils
        dataloader.py
        utils.py
│||||||||||||||||||||||||| Model Related         
```

**Fake News Detection Model quoted from**

 [M3DFEND](https://github.com/ictmcg/m3fend)

 [Paper](https://ieeexplore.ieee.org/document/9802916)

**Reference**
```
@article{zhu2022memory,
  title={Memory-Guided Multi-View Multi-Domain Fake News Detection},
  author={Zhu, Yongchun and Sheng, Qiang and Cao, Juan and Nan, Qiong and Shu, Kai and Wu, Minghui and Wang, Jindong and Zhuang, Fuzhen},
  journal={IEEE Transactions on Knowledge and Data Engineering},
  year={2022},
  publisher={IEEE}
}
@inproceedings{nan2021mdfend,
  title={MDFEND: Multi-domain fake news detection},
  author={Nan, Qiong and Cao, Juan and Zhu, Yongchun and Wang, Yanyan and Li, Jintao},
  booktitle={Proceedings of the 30th ACM International Conference on Information \& Knowledge Management},
  pages={3343--3347},
  year={2021}
}
```