**Status:** Archive (code is provided as-is, no updates expected)


setup:
for gpu: set the environment variable "CUDA_VISIBLE_DEVICES"
export CUDA_VISIBLE_DEVICES=1

Version of gym: 0.10.5
install baseline of openai (from github, ojo: reinstall downgrade the version of gym to make it compatible with the code)º
## [Exploration by Random Network Distillation](https://arxiv.org/abs/1810.12894) ##


Yuri Burda*, Harri Edwards*, Amos Storkey, Oleg Klimov<br/>
&#42;equal contribution

OpenAI<br/>
University of Edinburgh


### Installation and Usage
The following command should train an RND agent on Montezuma's Revenge
```bash
python run_atari.py --gamma_ext 0.999
```
To use more than one gpu/machine, use MPI (e.g. `mpiexec -n 8 python run_atari.py --num_env 128 --gamma_ext 0.999` should use 1024 parallel environments to collect experience on an 8 gpu machine). 

### [Blog post and videos](https://blog.openai.com/reinforcement-learning-with-prediction-based-rewards/)
