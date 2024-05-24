# A principled distance-aware uncertainty quantification approach for enhancing the reliability of physics-informed neural network

In this project, we develop a principled uncertainty quantification approach to characterize the model uncertainty of PINN, and the estimated uncertainty is then exploited as an instructive indicator to identify collocation points where PINN produces a large prediction error. To this end, this paper seamlessly integrates spectral-normalized neural Gaussian process (SNGP) into PINN for principled and accurate uncertainty quantification. In the first step, we apply spectral normalization on the weight matrices of hidden layers in the PINN to make the data transformation from input space to the latent space distance-preserving. Next, the dense output layer of PINN is replaced with a Gaussian process to make the quantified uncertainty distance-sensitive. Afterwards, to examine the performance of different UQ approaches, we define several performance metrics tailored to PINN for assessing distance awareness in the measured uncertainty and the uncertainty-informed error detection capability. Finally, we employ three representative physical problems to verify the effectiveness of the proposed method in uncertainty quantification of PINN and compare the developed approach with Monte Carlo (MC) dropout using the developed performance metrics. Computational results suggest that the proposed approach exhibits a superior performance in improving the prediction accuracy of PINN and the estimated uncertainty serves as an informative indicator to detect PINN’s prediction failures.

## Getting Started

* The source codes of the four numerical examples are saved in three separate folders: **Example 1 pedagogical example**, **Example 2 heat equation**, **XX**, and **XX**.


## Requirements
* Python >= 3.6 (Anaconda3 is recommended)

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the required packages.

```bash
pip install -r requirements.txt
```

## Reference
If you find our program useful for your work, we kindly request that you cite the following work. 
```
@article{li2024principled,
  title={A principled distance-aware uncertainty quantification approach for enhancing the reliability of physics-informed neural network},
  author={Li, Jinwu and Long, Xiangyun and Deng, Xinyang and Jiang, Wen and Zhou, Kai and Jiang, Chao and Zhang, Xiaoge},
  journal={Reliability Engineering \& System Safety},
  volume={245},
  pages={109963},
  year={2024},
  publisher={Elsevier}
}
```