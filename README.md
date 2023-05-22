# **EM-Generator-Docking Users Guidance** #
Docking based molecular generation module (suitable for fused-ring nitro compounds). 

## Author: ##
- **Dr. Jian Liu**, liujian-12@caep.cn, Institute of Chemical Materials, CAEP
## Activation: ##
1. EM-Generator-Docking requires offline activation before use. 
2. The first run will generate 'sn.txt', then send it to liujian-12@caep.cn to ask for the activation file 'register.bin'.
## Requirements:  ##
1. ananconda
2. python 3.8
3. rdkit 2022.9.5
4. pandas 1.4.3
5. numpy 1.24.3
6. base64
7. hashlib
8. pyDes
9. psutil
## Usage: ##

    usage: EM_Generator_Docking.py [-h] [-s SKELETON] [-m] [-n NUMSUB]
    
    optional arguments:
      -h, this help message and exit
      -s, skeleton(mol), abs path required
      -m, dump mol files
      -n, substitution number
**Warning:** *Please remove the H atom of the skeleton in the mol file, and the retained H atom will not be replaced by substituents.*
## Example: ##
    python EM_Generator_Docking.py -s Examples/MYX_AB.mol -m

*The results will be written to the same directory of the skeleton path.*
