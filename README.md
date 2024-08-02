# hdrl-fp

This is the source code folder for the research project published on Nature Communications: https://www.nature.com/articles/s41467-024-50531-6/figures/3

## structure
1. `en_array`: energy landscape mesh from DFT
2. `run_configs`: configs for different environments
3. `single_agent_one_atom`: src for one atom scenario
4. `single_agent_two_atom`: src for two atom scenario
5. `scripts`: example running scripts 

## installation
1. setup GPU environment and install `warpdrive` package as instructed
2. under the root directory of `rlchemists`, run `bash setenv.sh` to setup the Python path for this project

## CUDA kernel for environment
Please contact the [authors](tian.lan@salesforce.com) for the kernel functions. The kernel functions are proprietary and are not yet open sourced for now. The code needs kernel functions to run the GPU mode.
   
## run
We simply choose the environment and type to run a particular training, the supported ones are all included
in the `run_configs` folders, for example, `run_configs/single_agent_one_atom_diffusion2d` can be run by 
`python example_training_script_numba.py --env single_agent_one_atom --type diffusion2d`

## cite
If you're using this study in your research or applications, please cite using this BibTeX:
```
@article{lan2024,
  title  = {Enabling high throughput deep reinforcement learning with first principles to investigate catalytic reaction mechanisms.},
  author = {Lan, Tian and Wang, Huan and An, Qi},
  year   = 2024,
  journal = {Nature Communications},
  volume  = {15},
  number  = {6281},
}
```
