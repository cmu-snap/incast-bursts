# Understanding Incast Bursts in Modern Datacenters, IMC 2024

This repo contains the source code and data for the simulation study (Section 4) in this paper:

_Christopher Canel, Balasubramanian Madhavan, Srikanth Sundaresan, Neil Spring, Prashanth Kannan, Ying Zhang, Kevin Lin, and Srinivasan Seshan. 2024. Understanding Incast Bursts in Modern Datacenters. In Proceedings of the 2024 ACM on Internet Measurement Conference (IMC '24). Association for Computing Machinery, New York, NY, USA, 674–680. https://doi.org/10.1145/3646547.3689028_

BibTex citation:
```
@inproceedings{10.1145/3646547.3689028,
  author = {Canel, Christopher and Madhavan, Balasubramanian and Sundaresan, Srikanth and Spring, Neil and Kannan, Prashanth and Zhang, Ying and Lin, Kevin and Seshan, Srinivasan},
  title = {Understanding Incast Bursts in Modern Datacenters},
  year = {2024},
  isbn = {9798400705922},
  publisher = {Association for Computing Machinery},
  address = {New York, NY, USA},
  url = {https://doi.org/10.1145/3646547.3689028},
  doi = {10.1145/3646547.3689028},
  booktitle = {Proceedings of the 2024 ACM Internet Measurement Conference},
  pages = {674–680},
  numpages = {7},
  keywords = {congestion control, datacenter networks, incast, microbursts, tcp},
  location = {Madrid, Spain},
  series = {IMC '24}
}
```


## Instructions to reproduce simulation results

Set up the repo and dependencies.
```bash
git clone https://github.com/cmu-snap/incast-bursts.git
cd incast-bursts
git submodule update --init
cd ns-3-dev-git/scratch
sudo apt update
sudo apt install cmake parallel
```

Run experiments. This will automatically build NS-3. Cmake will alert you to any missing dependencies. After the build, the experiments should take about 4 minutes to complete. In this example, results are stored in `~/incast_bursts_imc_experiments_data`.
```bash
./imc_experiments.sh ~/incast_bursts_imc_experiments_data
```

Produce graphs.
```bash


```


## Examine results without rerunning simulations

If you prefer to not run the experiments and simply want to view the data, the output files and graphs are stored in this repo in `incast_bursts_imc_experiments_data.tar.gz`. Simply untar this archive.
```bash
tar -xf incast_bursts_imc_experiments_data.tar.gz
```
