Environment:

For pretrained weights and python package dependencies, see

https://github.com/ashawkey/stable-dreamfusion

https://github.com/zhan-xu/RigNet

Test environment:

Ubuntu 22 with python=3.7 & torch 1.12 & CUDA 11.3 on a V100.

Attention:

1. Download several packages by hand:
https://pytorch-geometric.com/whl/torch-1.12.0%2Bcu113.html
2. "apt install xvfb" to avoid error caused by lack of GUI display
3. There will be a trival exception in stable-dreamfusion part(assert xxx), which can be easily fixed
4. If there is some problem about rtree, pip uninstall&install rtree



usage:

python main.py --text "a running thin man" --workspace trial -O

python main.py --workspace trial -O --test

python main.py --workspace trial -O --test --save_mesh

python quick_start.py

python maya_save_fbx.py  //save .obj and .mtl in advance
