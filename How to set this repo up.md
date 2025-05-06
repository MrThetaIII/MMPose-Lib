# How to set this up?

## Step 1: Virtual Env with python 3.8

```shell
conda create --name openmmlab python=3.8 -y
```

## Step 2: Correct virsion of PyTorch

```shell
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

you can test with:

```shell
python torch_test.py
```

## Step 3: Openmim

```shell
pip install -U openmim
```

## Step 4: Install mmpose

```shell
pip install mmengine==0.10.7
pip install mmcv==2.1.0
pip install mmdet==3.3.0
pip install -r requirements.txt
pip install -v -e .
```

## Step 5: Download the demo files

```shell
mim download mmpose --config td-hm_hrnet-w48_8xb32-210e_coco-256x192  --dest .
```

## Step 6: Run the demo

Now do your self a favor and get to the cmd instead of power shell. No luck for linux users. Sorry Jemmy. Run the command within the file.

```shell
demo.bat
```
