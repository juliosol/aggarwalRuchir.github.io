**Status:** Archive (code is provided as-is, no updates expected)

## Multi-Step Curiosity Driven Learning ##
#### [[Project Website]](https://aggarwalruchir.github.io/) [[Demo Video]]()

Ruchir Aggarwal*, Kushantha U. Attanayake*, Dennis Li*, Julio Soldevilla*, Poorani Ravindhiran<br/>
(&#42; alphabetical ordering, equal contribution)

Computer Science and Engineering, University of Michigan<br/>
Mathematics, University of Michigan<br/>
Robotics, University of Michigan

<a href="https://aggarwalruchir.github.io/">
<img src="" width="500">
</img></a>

This is a TensorFlow based implementation for our [paper on multi-step curiosity driven learning](https://aggarwalruchir.github.io/EECS598_012_Final_Report.pdf) across 4 environments. 
Curiosity is a type of intrinsic reward function which uses prediction error as reward signal. In this paper, we extend the 
work done by [Deepak Pathak et al.](https://pathak22.github.io) and investigate the effects of generating multiple step predictions into the future, and 
using all predictions in our definition of curiosity. We perform experiments with different weight combinations for multiple 
step predictions and present our results. We restrict ourselves to 4 environments due to limited resources and extensive 
training time for each environment.

### Installation and Usage
The following command should train a pure exploration agent on Mario with default experiment parameters.
```bash
python run.py
```
To use more than one gpu/machine, use MPI (e.g. `mpiexec -n 8 python run.py` should use 1024 parallel environments to collect experience instead of the default 128 on an 8 gpu machine). 

### Other helpful pointers
- [Original Paper](https://pathak22.github.io/large-scale-curiosity/resources/largeScaleCuriosity2018.pdf)



