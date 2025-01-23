
<h1 align="center">
  <!-- <br>
  <a href="http://www.amitmerchant.com/electron-markdownify"><img src="https://raw.githubusercontent.com/amitmerchant1990/electron-markdownify/master/app/img/markdownify.png" alt="Markdownify" width="200"></a>
  <br> -->
  🔥 One-Prompt-One-Story: Free-Lunch Consistent Text-to-Image Generation Using a Single Prompt
  <br>
</h1>


<div align="center">

[![demo](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Online_Demo-blue)]()&nbsp;
[![arXiv](https://img.shields.io/badge/arXiv%20paper-2406.06525-b31b1b.svg)]()&nbsp;
[![project page](https://img.shields.io/badge/Project_page-More_visualizations-green)]()&nbsp;

</div>



<p align="center">
  <a href="#key-features">Key Features</a> •
  <a href="#how-to-use">How To Use</a> •
  <a href="#license">License</a> •
  <a href="#Citation">Citation</a> 
</p>

<p align="center">
  <img src="./resource/photo.gif" alt="screenshot" />
</p>


## Key Features

* Consistent Identity Image Generation.
* Gradio Demo.
* Consistory+ Benchmark: contains 200 prompt sets, with each set containing between 5 and 10 prompts, categorized into 8 superclasses: humans, animals, fantasy, inanimate, fairy tales, nature, technology.
* Benchmark Generation Code.


## How To Use

To clone and run this application, you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
$ git clone https://github.com/byliutao/1Prompt1Story

# Go into the repository
$ cd 1Prompt1Story

### Install dependencies ###
$ conda create --name 1p1s python=3.10
$ conda activate 1p1s
# choose the right cuda version of your device
$ conda install pytorch torchvision torchaudio pytorch-cuda=12.1 -c pytorch -c nvidia 
$ conda install conda-forge::transformers 
$ conda install -c conda-forge diffusers
$ pip install opencv-python scipy gradio=4.44.1 sympy==1.13.1
### Install dependencies ENDs ###

# Run sample code
$ python main.py

# Run gradio demo
$ python app.py

# Run Consistory+ benchmark
$ python -m resource.gen_benchmark --save_dir ./result/benchmark --benchmark_path ./resource/consistory+.yaml
```

> **Note**
> If you're using Linux Bash for Windows, [see this guide](https://www.howtogeek.com/261575/how-to-run-graphical-linux-desktop-applications-from-windows-10s-bash-shell/) or use `node` from the command prompt.


## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## Citation
If our work assists your research, feel free to give us a star ⭐ or cite us using:
```
arixv
```