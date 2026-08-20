# Recursos Adicionales

## Herramientas

- PyTorch Documentation: <https://pytorch.org/docs/>
- PyTorch Distributed: <https://pytorch.org/docs/stable/distributed.html>
- NVIDIA Developer: <https://developer.nvidia.com/>
- Slurm Documentation: <https://slurm.schedmd.com/>

## Recursos de datasets libres

- [Kaggle Datasets](https://www.kaggle.com/datasets)
- [UCI machine learning](https://archive-ics-uci-edu.translate.goog/?_x_tr_sch=http&_x_tr_sl=en&_x_tr_tl=es&_x_tr_hl=es&_x_tr_pto=tc)
- [Google dataset search](https://datasetsearch.research.google.com/)
- [Mendeley data](https://data.mendeley.com/)
- [Awesome Public Datasets](https://github.com/awesomedata/awesome-public-datasets)
- [Open data AWS](https://registry.opendata.aws/)
- [Datos abiertos Colombia](https://www.datos.gov.co/)


## 🗃️ Paquetes y librerías


### Docker environments
A preconfigured environment has been provided to ensure that all code runs with the correct dependencies. This helps maintain reproducibility and avoids issues related to package versions or system configuration. To use this environment, you must first install Docker. You can follow the official installation guide here: 

[https://docs.docker.com/engine/install/](https://docs.docker.com/engine/install/)

Once Docker is installed, download the container image by running the containers

List of containers: 


| Name | Description | Download | Run |
|---|---|---|---|
| ```jupyter-ml-docker```| Jupyter server running essential ML libraries and dependencies | ```docker pull rubenfonnegra/jupyter-ml-docker``` | ```docker run -p 8888:8888 rubenfonnegra/jupyter-ml-docker``` |
|```sem-db-docker```| Jupyter server running libraries for basic data analysis | ```docker pull rubenfonnegra/sem-db-docker``` | ```docker run -p 8888:8888 rubenfonnegra/sem-db-docker``` |
|```pytorch_docker_r```| Jupyter server running pytorch with GPU support | ```docker pull rubenfonnegra/pytorch_docker_r``` | ```docker run -it --rm rubenfonnegra/pytorch_docker_r /bin/bash``` |

NOTE: JupyterLab instances are accessible from your browser. From there, you can upload the notebook files and execute the code within the prepared environment. Once the container is running, open the URL shown in the terminal to open your browser and navigate through the files. 


## Bibliografía

### Libros

- Hager, G., & Wellein, G. (2010). *Introduction to High Performance Computing for Scientists and Engineers*. CRC Press.

- Kirk, D. B., & Hwu, W. W. (2022). *Programming Massively Parallel Processors: A Hands-on Approach* (4th ed.). Morgan Kaufmann.

- Pacheco, P., & Malensek, M. (2021). *An Introduction to Parallel Programming* (2nd ed.). Morgan Kaufmann.

- Grama, A., Gupta, A., Karypis, G., & Kumar, V. (2003). *Introduction to Parallel Computing* (2nd ed.). Addison-Wesley.

- Hennessy, J. L., & Patterson, D. A. (2019). *Computer Architecture: A Quantitative Approach* (6th ed.). Morgan Kaufmann.

- Golub, G. H., & Van Loan, C. F. (2013). *Matrix Computations* (4th ed.). Johns Hopkins University Press.

- Leskovec, J., Rajaraman, A., & Ullman, J. D. (2020). *Mining of Massive Datasets* (3rd ed.). Cambridge University Press. <http://www.mmds.org/>


### Artículos y papers

- Amdahl, G. M. (1967). *Validity of the Single Processor Approach to Achieving Large Scale Computing Capabilities*. AFIPS Spring Joint Computer Conference.

- Gustafson, J. L. (1988). *Reevaluating Amdahl's Law*. Communications of the ACM, 31(5), 532–533.

- Williams, S., Waterman, A., & Patterson, D. (2009). *Roofline: An Insightful Visual Performance Model for Multicore Architectures*. Communications of the ACM, 52(4), 65–76.

- Halko, N., Martinsson, P. G., & Tropp, J. A. (2011). *Finding Structure with Randomness: Probabilistic Algorithms for Constructing Approximate Matrix Decompositions*. SIAM Review, 53(2), 217–288.

- Shoeybi, M., et al. (2019). *Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism*. arXiv.

- Huang, Y., et al. (2019). *GPipe: Efficient Training of Giant Neural Networks Using Pipeline Parallelism*. Advances in Neural Information Processing Systems (NeurIPS).

- Rajbhandari, S., Rasley, J., Ruwase, O., & He, Y. (2020). *ZeRO: Memory Optimizations Toward Training Trillion Parameter Models*. SC20: International Conference for High Performance Computing, Networking, Storage and Analysis.

- Li, S., et al. (2020). *PyTorch Distributed: Experiences on Accelerating Data Parallel Training*. Proceedings of the VLDB Endowment.


### GPU Computing y CUDA

- NVIDIA. *CUDA Documentation*. <https://docs.nvidia.com/cuda/>

- NVIDIA. *CUDA C++ Programming Guide*. <https://docs.nvidia.com/cuda/cuda-c-programming-guide/>

- NVIDIA. *CUDA Developer Resources*. <https://developer.nvidia.com/cuda>

- NVIDIA. *An Even Easier Introduction to CUDA*. <https://developer.nvidia.com/blog/even-easier-introduction-cuda/>

- NVIDIA. *CUDA Samples*. <https://github.com/NVIDIA/cuda-samples>



### Repositorios y recursos prácticos

- PyTorch. *Distributed Communication Package*.  
  <https://pytorch.org/docs/stable/distributed.html>

- PyTorch. *Distributed Overview*.  
  <https://docs.pytorch.org/tutorials/beginner/dist_overview.html>

- PyTorch. *Distributed Data Parallel Tutorial*.  
  <https://docs.pytorch.org/tutorials/intermediate/ddp_tutorial.html>

- PyTorch. *Distributed Training Tutorials*.  
  <https://docs.pytorch.org/tutorials/distributed.html>

- DeepSpeed. *Deep Learning Optimization Library*.  
  <https://www.deepspeed.ai/>

- PyTorch Examples.  
  <https://github.com/pytorch/examples>

- PyTorch Tutorials.  
  <https://github.com/pytorch/tutorials>

- NVIDIA CUDA Samples.  
  <https://github.com/NVIDIA/cuda-samples>
