# train-data

Process to train a theme:
- go to the folder in midjourney
- run the extension, it will automatically download all images (if you have multiple themes, do not forget to refresh every time)
- after this, locate all the theme_name.csv files in g:/midjourney thmes/files folder
- run script.py, it will generate folders name_final,
- remove final from all folder names,
- upload all folders to aws dashbaord
- now run caption.py after locating all these folders into data folder
- this will generate caption_file.zip files inside results folder
- copy these files to train-data local git repo clone
- git push
- copy the dictionary output by caption.py
- run Manu's copy of replicate-training in colab by train unstudio account
- run first 2 cells, skip 3rd then in 4th, copy-paste he dictionary, then run
- wait for around 15-20 minutes, during this, check replicate
- during training, create templates in aws dashboard
- get the weights.tar in output cell,
- copy the weights to aws dashboard lora section
