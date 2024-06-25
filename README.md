## Download Open Images Dataset(Annotated)

## Create a virtual env
conda create -n DL_DownloadImages python=3.10

### actaivate the virtual env
conda activate DL_DownloadImages

## Install the requrienments
pip install -r .\requirements.txt

## Donwload Images
python main.py downloader --classes Balloon Airplane --type_csv train --limit 400

## To downoad images in a single folder
python main.py downloader --classes Balloon Airplane --type_csv train --limit 400 --multiclasses 1

## Convert Annotations
python convert_annotations.py