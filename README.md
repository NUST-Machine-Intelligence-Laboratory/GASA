# A Hybrid Approach for Fine-Grained Cross-Media Retrieval
## Introduction
This is the Pytorch implementation for our paper: **A Hybrid Approach for Fine-Grained Cross-Media Retrieval**
## Network Architecture
The architecture of our proposed approach is as follows
![](https://github.com/NUST-Machine-Intelligence-Laboratory/GASA/blob/main/fig/architecture.png)
## Installation
**Requirement**  
* pytorch, tested on [v1.0]  
* CUDA, tested on v9.0  
* Language: Python 3.6
## How to use
The code is currently tested only on GPU.
* **Download dataset**  
Please visit [dataset](http://59.108.48.34/tiki/FGCrossNet/).
* **Prepare audio data**  
python audio.py
* **Training**  
   * If you want to train the whole model from beginning using the source code, please follow the subsequent steps.
      * Download dataset to the ```dataset``` folder.
      * In ```main_gan_lstm_resnet.py```  
      >* modify ```lr in params1``` to ```0.001```, ```lr in params2``` and ```lr in discriminator``` to ```1```.  
      >* modify ```model_path``` to the path where you want to save your parameters of networks.
      * Activate virtual environment (e.g. conda) and then run the script  
      ```python
      python main_gan_lstm_resnet.py
      ```
* **Testing**  
   * If you just want to do a quick test on the model and check the final retrieval performance, please follow the subsequent steps.
      * The trained models of our work can be downloaded from [Baidu Cloud](https://pan.baidu.com/s/1ZiXq4nLhaD6vpOpTmSn_xA), and the extraction code is v99c.
      * Activate virtual environment (e.g. conda) and then run the script  
      ```python
      python test_gan.py
      ```

* **Results**
 The final experimental results are shown in the following table：
 ![](https://github.com/NUST-Machine-Intelligence-Laboratory/GASA/blob/main/fig/table.png)
 ![](https://github.com/NUST-Machine-Intelligence-Laboratory/GASA/blob/main/fig/figure5.png)
 ![](https://github.com/NUST-Machine-Intelligence-Laboratory/GASA/blob/main/fig/figure6.png)
 
