  
# 実行環境  
- python 3.10  
- cuda 11.3  
moduleをloadしておくこと  

# 実行環境セットアップ  
1. クローンする  
2. poetry install でライブラリをインストール  
3. stable-diffusionの重みファイルを下記コマンドでダウンロード  
	```
	wget -c https://huggingface.co/CompVis/stable-diffusion-v-1-4-original/resolve/main/sd-v1-4.ckpt  
	mkdir -p  models/ldm/stable-diffusion-v1  
	mv sd-v1-4.ckpt models/ldm/stable-diffusion-v1/model.ckpt  
	```  

# テストコマンド  
```
python mist_v3.py -img test/sample.png --output_name misted_sample  
```
