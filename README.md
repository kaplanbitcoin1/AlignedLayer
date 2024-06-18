- Sunucumuzu güncelleyelim


#

```console
sudo apt update -y && sudo apt upgrade -y

```
#

- Gerekli dosyaları yükleyelim

```console

curl -L https://raw.githubusercontent.com/yetanotherco/aligned_layer/main/batcher/aligned/install_aligned.sh | bash
source /root/.bashrc

```
#

- Proof test dosyasını çekelim

```console

curl -L https://raw.githubusercontent.com/yetanotherco/aligned_layer/main/batcher/aligned/get_proof_test_files.sh | bash
```

- Bu kısmı tek komut halinde girelim

```console
rm -rf ~/aligned_verification_data/ &&
aligned submit \
--proving_system SP1 \
--proof ~/.aligned/test_files/sp1_fibonacci.proof \
--vm_program ~/.aligned/test_files/sp1_fibonacci-elf \
--aligned_verification_data_path ~/aligned_verification_data \
--conn wss://batcher.alignedlayer.com
```

- Verilen çıktıyı ss alıp, tx url'sini Twitter'da AlignedLayer'i etiketleyerek paylaşalım.
  
- Aligned Discord adresine gidip testnet bölümünde paylaştığımız twitter gönderisinin linkini burada paylaşalım. 

- İşlemler bu kadar.
