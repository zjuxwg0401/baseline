# Baseline
Baseline for [1st Anti-UAV Challenge](https://anti-uav.github.io).

<div align="center">
  <img src="anti-uav.gif" width="600px" />
</div>

## Download Dataset `test-dev`
- [Google Drive](https://drive.google.com/open?id=1GICr5e9CZN0tcFM_VXhyogzxWD3LMvAw)
- [Baidu Yun](https://pan.baidu.com/s/1dJR0VKyLyiXBNB_qfa2ZrA)(sagx)
 
**Note**: 
- We provide IR, RGB videos and their ground-truth labels. Contestants can only use both IR and RGB videos and **their location in the first frame**.
Our evaluation ranks are calculated according to the results on the IR video.
- Update: (2020/02/19) upload IR_label.json 


## Test
- set up the environment
```shell
conda create -n anti_uav python=3.7
conda activate anti_uav
pip install opencv-python torch
```
- run
```shell
python test.py
```
- You will see the following results.
    
```shell
[001/100]  20190925_131530_1_4    IR Fixed Measure: 0.187
[002/100]  20190926_183400_1_8    IR Fixed Measure: 0.788
...
[100/100]  20190925_213001_1_2    IR Fixed Measure: 0.028
[Overall]    IR Mixed Measure: 0.420
```
