<a id="readme-top"></a>

<!-- PROJECT LOGO -->

<div align="center">
  <h1><img src="assets/ImmunoStruct_cover.png" width="200"><br><code>ImmunoStruct</code></h1>
  <h3>ImmunoStruct enables multimodal deep learning for immunogenicity prediction</h3>

  [![nature](https://img.shields.io/badge/nature_machine_intelligence-gold)](https://www.nature.com/articles/s42256-025-01163-y)
  [![PDF](https://img.shields.io/badge/PDF-DADBDD)](https://www.nature.com/articles/s42256-025-01163-y.pdf)
  ![Python](https://img.shields.io/badge/Python-3.8-3776ab)
  ![PyTorch](https://img.shields.io/badge/PyTorch-2.1.2-ee4c2c)
  [![GitHub Stars](https://img.shields.io/github/stars/KrishnaswamyLab/ImmunoStruct.svg?style=social\&label=Stars)](https://github.com/KrishnaswamyLab/ImmunoStruct)
  <br>[![LinkedIn](https://img.shields.io/badge/LinkedIn-Kevin-blue)](https://www.linkedin.com/in/kevin-bijan-givechian-phd-36467ba3/)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Joao-blue)](https://www.linkedin.com/in/joao-felipe-rocha/)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Chen-blue)](https://www.linkedin.com/in/chenliu1996/)
  <br>[![Twitter Follow](https://img.shields.io/twitter/follow/Kevin.svg?style=social)](https://x.com/KevinGivechian)
  [![Twitter Follow](https://img.shields.io/twitter/follow/Chen.svg?style=social)](https://x.com/ChenLiu_1996)
  [![Twitter Follow](https://img.shields.io/twitter/follow/KrishnaswamyLab.svg?style=social)](https://x.com/KrishnaswamyLab)
</div>

In case you don't have access to Nature, here are the [main paper](pdf/ImmunoStruct_NMI.pdf) and the [supplementary materials](pdf/ImmunoStruct_NMI_supp.pdf).

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#news">News</a>
    </li>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#key-features">Key Features</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#citation">Citation</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#model-architecture">Model Architecture</a></li>
    <li><a href="#troubleshooting">Troubleshooting</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

## News

News in English<br>
[![news](https://img.shields.io/badge/news-Decoding_Bio-DADBDD)](https://decodingbio.substack.com/p/biobyte-144-a-virtual-model-of-cell)
[![news](https://img.shields.io/badge/news-Bioengineer-DADBDD)](https://bioengineer.org/immunostruct-advancing-deep-learning-in-immunogenicity-prediction/)
[![news](https://img.shields.io/badge/news-GeneOnline-DADBDD)](https://www.geneonline.com/deep-learning-model-immunostruct-developed-to-improve-prediction-of-immunogenic-epitopes-for-vaccine-research/)
<br>[![wiki](https://img.shields.io/badge/wiki-Wikipedia_Immunogenicity-pink)](https://en.wikipedia.org/wiki/Immunogenicity)


News in Chinese<br>
[![news](https://img.shields.io/badge/news-新智元@网易-gold)](https://www.163.com/dy/article/KJ13HJ340511ABV6.html)
[![news](https://img.shields.io/badge/news-腾讯云_(Tencent_Cloud)-DADBDD)](https://cloud.tencent.com/developer/article/2612794)
<br>[![news](https://img.shields.io/badge/news-新智元@搜狐-F6E7B2)](https://m.sohu.com/a/974949014_473283)
[![news](https://img.shields.io/badge/news-新智元@智源社区-F6E7B2)](https://hub.baai.ac.cn/view/51813)
[![news](https://img.shields.io/badge/news-新浪财经_转发_新智元-F6E7B2)](https://finance.sina.com.cn/stock/t/2026-01-11/doc-inhfxvtm9135944.shtml)
[![news](https://img.shields.io/badge/news-AI中文社_转发_新智元-F6E7B2)](https://www.aizws.net/news/detail/6922)
[![news](https://img.shields.io/badge/news-百度_转发_新智元-F6E7B2)](https://baijiahao.baidu.com/s?id=1854022994702774585)
<br>[![wiki](https://img.shields.io/badge/wiki-百度百科_免疫原性-pink)](https://baike.baidu.com/item/%E5%85%8D%E7%96%AB%E5%8E%9F%E6%80%A7/5292060)
[![wiki](https://img.shields.io/badge/wiki-百度百科_图神经网络-pink)](https://baike.baidu.com/item/%E5%9B%BE%E7%A5%9E%E7%BB%8F%E7%BD%91%E7%BB%9C/59091829)


&#9744; TODO: create and release an end-to-end tool.
<br>&#9744; TODO: verify, document and release the multimodal dataset, likely after the ICML deadline.
<br>&#x2705; Dec 31, 2025: **[Published](https://www.nature.com/articles/s42256-025-01163-y) in Nature Machine Intelligence.**
<br>&#x2705; Dec 04, 2025: Informally presented at NeurIPS 2025 (did not submit, no dual-submission concern).
<br>&#x2705; Aug 18, 2025: Received the [Colton Innovation Fund](https://ventures.yale.edu/news/yales-colton-center-autoimmunity-announces-2025-awardees-advancing-innovation-autoimmune) from [Colton Center for Autoimmunity at Yale University](https://ventures.yale.edu/colton-center-for-autoimmunity).
<br>&#x2705; May 06, 2025: Submitted to Nature Machine Intelligence.
<br>&#x2705; Nov 05, 2024: Presented at MoML@MIT 2024 (non-archival abstract & poster).
<br>&#x2705; Nov 01, 2024: [Preprint](https://www.biorxiv.org/content/10.1101/2024.11.01.621580) released.

<!-- ABOUT THE PROJECT -->
## About The Project

<div align="center">
  <img src="assets/schematic.png" alt="ImmunoStruct Architecture" width="800">
</div>

ImmunoStruct is a multimodal deep learning framework that integrates sequence, structural, and biochemical information to predict multi-allele class-I peptide-MHC immunogenicity. By leveraging multimodal data from 26,049 peptide-MHCs and jointly modeling sequence and structure, ImmunoStruct significantly improves immunogenicity prediction performance for both infectious disease epitopes and cancer neoepitopes.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Key Features

* **Multimodal Integration**: Combines peptide-MHC protein sequence, structure, and biochemical properties
* **Novel Cancer-Wildtype Contrastive Learning**: Enhances specificity for cancer neoepitope detection
* **Enhanced Interpretability**: Provides insights into the substructural basis of immunogenicity

<div align="center">
  <img src="assets/contrastive_learning.png" alt="Contrastive Learning Approach" width="800">
  <img src="assets/visualizations.png" alt="Visualizations" width="800">
</div>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CITATION -->
## Citation

If you use ImmunoStruct in your research, please cite our paper:

BibTeX:
```bibtex
@article{givechian2026immunostruct,
  title={ImmunoStruct enables multimodal deep learning for immunogenicity prediction},
  author={Givechian, Kevin Bijan and Rocha, Jo{\~a}o Felipe and Liu, Chen and Yang, Edward and Tyagi, Sidharth and Greene, Kerrie and Ying, Rex and Caron, Etienne and Iwasaki, Akiko and Krishnaswamy, Smita},
  journal={Nature Machine Intelligence},
  volume={8},
  pages={70--83},
  year={2026},
  publisher={Nature Publishing Group UK London}
}
```
Nature format:<br>
Givechian, K.B., Rocha, J.F., Liu, C. et al. ImmunoStruct enables multimodal deep learning for immunogenicity prediction. *Nat Mach Intell* 8, 70–83 (2026). https://doi.org/10.1038/s42256-025-01163-y


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

To get ImmunoStruct up and running locally, follow these steps.

### Pre-requisites

Before installation, ensure you have:
* Python 3.8+
* CUDA-compatible GPU (recommended)
* Conda package manager
* Weights & Biases account for experiment tracking

### Dependencies
- python 3.8
- torch 2.1.2
- dgl
- torch_geometric 2.5.3

### Installation

1. **Clone the repository**
   ```sh
   git clone https://github.com/KrishnaswamyLab/ImmunoStruct.git
   cd ImmunoStruct
   ```

2. **Create and activate conda environment**
   ```sh
   conda create --name immuno python=3.8 -c anaconda -c conda-forge -y
   conda activate immuno
   ```

3. **Install core dependencies**
   ```sh
   conda install cudatoolkit=11.2 wandb pydantic -c conda-forge -y
   conda install scikit-image pillow matplotlib seaborn tqdm -c anaconda -y
   ```

4. **Install PyTorch**
   ```sh
   python -m pip install torch==2.1.2 torchvision==0.16.2 torchaudio==2.1.2 --index-url https://download.pytorch.org/whl/cu118
   ```

5. **Install DGL**
   ```sh
   python -m pip install dgl -f https://data.dgl.ai/wheels/torch-2.1/cu118/repo.html
   python -m pip install torchdata==0.7.1
   ```

6. **Install PyTorch Geometric and related packages**
   ```sh
   python -m pip install torch-scatter==2.1.2+pt21cu118 torch-sparse==0.6.18+pt21cu118 torch-cluster==1.6.3+pt21cu118 torch-spline-conv==1.2.2+pt21cu118 torch_geometric==2.5.3 numpy==1.21.1 -f https://data.pyg.org/whl/torch-2.1.2+cu118.html
   ```

7. **Install AlphaFold2-related packages**
   ```sh
   python -m pip install jax==0.2.25 jaxlib==0.1.69+cuda111 -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
   python -m pip install "alphafold-colabfold==2.0.0" "colabfold==1.2.0" "dm-haiku==0.0.4"
   python -m pip install "biopython==1.78"
   ```

   Go to /path/to/environment/lib/python3.8/site-packages/jaxlib/xla_client.py: change `np.object` to `object`.

   Go to /path/to/environment/lib/python3.8/site-packages/alphafold/common/residue_constants.py: change `np.int` to `np.int32`.

   Go to /path/to/environment/lib/python3.8/site-packages/alphafold/data/templates.py: change `np.object` to `object`.

8. **Install additional packages**
   ```sh
   python -m pip install graphein[extras]
   python -m pip install lifelines
   python -m pip install -U phate
   python -m pip install multiscale-phate
   ```

9. **Set up environment variables (if needed)**
   ```sh
   export LD_LIBRARY_PATH=/path/to/conda/envs/immuno/lib:$LD_LIBRARY_PATH
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

### Data Preparation

Place the following files in the `data/` folder:
- `ImmunoStruct_IEDB_data.csv`
- `ImmunoStruct_CEDAR_data_cancer.csv`
- `ImmunoStruct_CEDAR_data_wildtype.csv`
- `ImmunoStruct_clinical_data.csv`
- `ImmunoStruct_clinical_data_survival.csv`
- `HLA_allele_sequences.csv`


**Generate PyG graph files:**

These PyG graph files can be generated using the below command from the corresponding AlphaFold folders.
```sh
# Download colabfold and remember where it is downloaded to.
python -m colabfold.download

# Run the protein folding script.
cd immunostruct/preprocessing
python step1_sequence_to_pdb.py --input-csv ../../data/ImmunoStruct_clinical_data.csv --start 0 --end 5 --params-loc /gpfs/radev/home/cl2482/.cache/colabfold --peptide-col-index 1 --sequence-col-index 4

# Run the PDB-to-PyG conversion script.
python step2_pdb_to_pyg.py
```


### Training and Testing

1. **Set up Weights & Biases**

   Create a project on [Weights & Biases](https://wandb.ai/home) matching your project name.

2. **Run Experiments**
   ```sh
   # HybridModelv2 with full sequence and sequence loss
   python train_PropIEDB_PropCancer_ImmunoCancer.py --full-sequence --sequence-loss --model HybridModelv2 --wandb-username YOUR_WANDB_USERNAME

   # HybridModel with full sequence and sequence loss
   python train_PropIEDB_PropCancer_ImmunoCancer.py --full-sequence --sequence-loss --model HybridModel --wandb-username YOUR_WANDB_USERNAME

   # Sequence with fingerprint model
   python train_PropIEDB_PropCancer_ImmunoCancer.py --full-sequence --sequence-loss --model SequenceFpModel --wandb-username YOUR_WANDB_USERNAME

   # Sequence-only model
   python train_PropIEDB_PropCancer_ImmunoCancer.py --full-sequence --sequence-loss --model SequenceModel --wandb-username YOUR_WANDB_USERNAME

   # Structure-only model
   python train_PropIEDB_PropCancer_ImmunoCancer.py --full-sequence --model StructureModel --wandb-username YOUR_WANDB_USERNAME
   ```

3. **Our main experiments**
   ```sh
   # IEDB training
   python train_IEDB_wFT.py --full-sequence --model HybridModelv2 --wandb-username immunoteam --sequence-loss --seed 1

   # Cancer training
   python infer_IEDB_or_Cancer.py --model HybridModelv2_Comparative --full-sequence --infer_dataset Cancer --comparative --use-wt-for-downstream --seed 1

   # IEDB or Cancer inference
   python infer_IEDB_or_Cancer.py --model HybridModelv2 --model-dir /path/to/model --model-filename MODEL_FILENAME --full-sequence --infer_dataset IEDB
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- TROUBLESHOOTING -->
## Troubleshooting

### Common Issues

**GLIBCXX Error**
```
ImportError: $some_path/libstdc++.so.6: version 'GLIBCXX_3.4.29' not found
```
**Solution:** Add your conda environment path to `LD_LIBRARY_PATH`:
```sh
export LD_LIBRARY_PATH=/path/to/conda/envs/immuno/lib:$LD_LIBRARY_PATH
```

**CUDA Compatibility Issues**
- Ensure your CUDA version matches the PyTorch installation
- Verify GPU availability with `torch.cuda.is_available()`

**Memory Issues**
- Reduce batch size in training scripts
- Use gradient checkpointing for large models

**Wandb Authentication**
- Login to Wandb: `wandb login`
- Ensure project names match between script and Wandb dashboard

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the Yale License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Krishnaswamy Lab - [@KrishnaswamyLab](https://twitter.com/KrishnaswamyLab)

Project Link: [https://github.com/KrishnaswamyLab/ImmunoStruct](https://github.com/KrishnaswamyLab/ImmunoStruct)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
[biorxiv-shield]: https://img.shields.io/badge/bioRxiv-ImmunoStruct-firebrick?style=for-the-badge
[biorxiv-url]: https://www.biorxiv.org/content/10.1101/2024.11.01.621580
[twitter-shield]: https://img.shields.io/twitter/follow/KrishnaswamyLab.svg?style=for-the-badge&logo=twitter&colorB=1DA1F2
[twitter-url]: https://twitter.com/KrishnaswamyLab
[stars-shield]: https://img.shields.io/github/stars/KrishnaswamyLab/ImmunoStruct.svg?style=for-the-badge
[stars-url]: https://github.com/KrishnaswamyLab/ImmunoStruct/stargazers
[issues-shield]: https://img.shields.io/github/issues/KrishnaswamyLab/ImmunoStruct.svg?style=for-the-badge
[issues-url]: https://github.com/KrishnaswamyLab/ImmunoStruct/issues
[license-shield]: https://img.shields.io/badge/license-Yale-blue.svg?style=for-the-badge
[license-url]: https://github.com/KrishnaswamyLab/ImmunoStruct/blob/master/LICENSE.txt
[PyTorch]: https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white
[PyTorch-url]: https://pytorch.org/
[PyG]: https://img.shields.io/badge/PyTorch_Geometric-3C2179?style=for-the-badge&logo=pytorch&logoColor=white
[PyG-url]: https://pytorch-geometric.readthedocs.io/
[DGL]: https://img.shields.io/badge/DGL-FF6B35?style=for-the-badge&logo=python&logoColor=white
[DGL-url]: https://www.dgl.ai/
[Wandb]: https://img.shields.io/badge/Weights_&_Biases-FFBE00?style=for-the-badge&logo=weightsandbiases&logoColor=white
[Wandb-url]: https://wandb.ai/
[Python]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white
[Python-url]: https://python.org/
[Conda]: https://img.shields.io/badge/Conda-44A833?style=for-the-badge&logo=anaconda&logoColor=white
[Conda-url]: https://conda.io/
