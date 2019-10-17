# imdb_multi_trainer

##prepare data

```shell
wget https://fleet.bj.bcebos.com/text_classification_data.tar.gz
tar -zxvf text_classification_data.tar.gz
```

##build

```shell
mkdir build
cd build
rm -rf *
PADDLE_LIB=path/to/your/fluid_inference_install_dir/
cmake .. -DPADDLE_LIB=$PADDLE_LIB  -DWITH_MKLDNN=OFF -DWITH_MKL=OFF
make
```
