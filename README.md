# Sylheti-Nagri-OCR

# Execution
* run **scripts/resource_gen.ipynb** with proper variable paths to generate:
    * Synthetic Grapheme based dictionary 
    * Single line vocab file *(such file are needed for synthtiger,EasyOCR etc)*
    * Multi line vocab file *(such file are needed for synthindic)*
    * Train data unique word based dictionary
    * Separates folds (train and test) and creates data.txt where absolute path of the image and label are tab separated 
    
* **Synthtiger**: [follow advanced usage section](https://github.com/clovaai/synthtiger/tree/master#advanced-usage) 
    * needed scripts are stored under **scripts/synthtiger**
    * **Font Customization**: 
        
        ```bash
        python scripts/synthtiger/extract_font_charset.py -w 1 /home/apsisdev/OCR/SylhetiNagri/fonts/
        ```
    
**System Info**:

```bash
OS          : Ubuntu 22.04.2 LTS x86_64 
Host        : Z490 GAMING X AX -CF 
Kernel      : 5.19.0-38-generic 
Shell       : bash 5.1.16 
DE          : GNOME 42.5 
CPU         : Intel i9-10900K (20) @ 5.300GHz 
GPU         : NVIDIA GeForce RTX 3090 
Memory      : 13503MiB / 32022MiB 
```

# TODO
- [x] github installation and configuration 
- [x] resource_gen documentation
- [ ] synthtiger generation
- [ ] synthindic generation
- [ ] tfrs2 records
- [ ] training notebook
- [ ] inference notebook
- [ ] evaluation on real data 