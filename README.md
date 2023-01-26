# LF_Transformer
## Library install
conda create -n lf_transformer python=3.8.8
conda activate lf_transformer

conda install pytorch==1.7.1 torchvision==0.8.2 cudatoolkit=10.1.243 numpy=1.19.2 -c pytorch -y
conda install cudnn=7.6.5 -c anaconda -y
pip install -r requirements.txt
conda install nodejs -y
jupyter labextension install @jupyter-widgets/jupyterlab-manager

pip install -r ./requirements.txt

## run
python ./bin/LF_transformer.py --force ./output/{dataset_name}/lf_transformer/tuned_reproduced_ours/{seed}.toml
