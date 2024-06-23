
# ALIGNEDLAYER PUBLIC PROOF TASK  


## Getting Srtarted 

```
sudo apt update -y
sudo apt upgrade -y
```

### Install curl 
```
sudo apt-get install curl -y
```

### Download ALignedProof 
```
curl -L https://raw.githubusercontent.com/yetanotherco/aligned_layer/main/batcher/aligned/install_aligned.sh | bash
```

```
source /root/.bashrc
```


### Download an example SP1 proof file with it's ELF file 

```
curl -L https://raw.githubusercontent.com/yetanotherco/aligned_layer/main/batcher/aligned/get_proof_test_files.sh | bash
```


### Sending proof 

```
rm -rf ~/aligned_verification_data/ &&
aligned submit \
--proving_system SP1 \
--proof ~/.aligned/test_files/sp1_fibonacci.proof \
--vm_program ~/.aligned/test_files/sp1_fibonacci-elf \
--aligned_verification_data_path ~/aligned_verification_data \
--conn wss://batcher.alignedlayer.com
```

use this code to get the log you will screenshot for your X post
```
aligned verify-proof-onchain \
--aligned-verification-data ~/aligned_verification_data/*.json \
--rpc https://ethereum-holesky-rpc.publicnode.com \
--chain holesky
```


Use the explorer link in CMD to check if verified and you'll also see below image. 


-------------
----------------------
### Tweet exactly as screenshot and Submit Proof in Dscord 




--------------------------
### Submit in Discord 


# JOIN DISCORD FROM PROFILE 
https://linktr.ee/AlignedLayer




