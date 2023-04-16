# AnimationCrazy-Video-Downloader

## Abstract

### 项目名称
动画疯视频下载器  
AnimationCrazy Video Downloader

### 项目介绍
一个通过Python编写的, 用于下载动画疯视频的下载器。  
（来自一个编程业余爱好者的拙劣作品）
A downloader for AnimationCrazy videos based on Python.

### 版权信息
本项目由ac-dl.py与[N_m3u8DL-RE](https://github.com/nilaoda/N_m3u8DL-RE)两部分组合而成。其中本项目的ac-dl.py以获取视频的密钥信息与整理命令为主, [N_m3u8DL-RE](https://github.com/nilaoda/N_m3u8DL-RE)在本项目中的作用为：被ac-dl.py调用, 代为“跑腿”, 负责视频的下载。在此向[nilaoda](https://github.com/nilaoda)与其开发的[N_m3u8DL-RE](https://github.com/nilaoda/N_m3u8DL-RE)项目表示感谢。本项目无任何商业用途, 仅为个人学习, 方便个人使用。但您在使用/转发此项目及使用其中的程序时, 仍应注意标明作者(我, CrymanChen)  
This project consists of two parts: ac-dl.py and [N_m3u8DL-RE](https://github.com/nilaoda/N_m3u8DL-RE). The ac-dl.py focuses on obtaining video key information and sorting commands, while [N_m3u8DL-RE](https://github.com/nilaoda/N_m3u8DL-RE) is called by ac-dl.py and responsible for video downloading. I would like to express my gratitude to [nilaoda](https://github.com/nilaoda) and the [N_m3u8DL-RE](https://github.com/nilaoda/N_m3u8DL-RE) project for their contributions to this project. This project is intended solely for personal learning and convenience and has no commercial purpose. However, if you use or distribute this project or any of its scripts, please be sure to credit the author (CrymanChen).

## Usage (Chinese Simplified)
### 步骤说明
1. 解压压缩包, 将必要资源解压至文件夹内。  
![20230416202911](https://user-images.githubusercontent.com/106590233/232310013-0c75ba6d-2908-412f-b2a7-f6376fd2421a.png)  
2. `pip install -r requirements.txt`  
(此步骤默认情况下不需要进行, 可直接跳转至第3步, 如果遇到Python第三方库未安装等问题可退回至本步骤)  
3. `ac-dl.py`  
![20230416203109](https://user-images.githubusercontent.com/106590233/232310102-03e4dfac-6b2b-4acb-a474-9f02fe7eec17.png)  
4. 依次输入a. m3u8链接地址 b. 密钥地址 c. sn号  
![20230416203356](https://user-images.githubusercontent.com/106590233/232310738-6cbd215a-a069-44b7-aa5e-289d96b772cc.png)  
5. 等待视频下载完毕  
![20230416203628](https://user-images.githubusercontent.com/106590233/232311382-f63f8f3c-df0e-4c9d-81e9-41a9aeccc0bf.png)  
  
### 补充
1. 并非所有的视频都采用了“iv偏移”, 故当这种情况出现时, 程序会给出提示“未找到初始偏移向量”, 但该提示与下载失败非充要条件。  
例如下图中, 该视频无iv, 但最终仍然下载成功, “未找到初始偏移向量”仅为提示用。  
![20230416204444](https://user-images.githubusercontent.com/106590233/232312379-31ff35e7-0722-4161-a2f2-002ea3859464.png)
2. 在本项目中出现的“sn号匹配”检测仅为二次核对, 以免因输入错误导致下载失败。
