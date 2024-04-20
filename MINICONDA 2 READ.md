These four commands quickly and quietly install the latest 64-bit version of the installer and then clean up after themselves. To install a different version or architecture of Miniconda for Linux, change the name of the .sh installer in the wget command.

mkdir -p ~/[folder of your choice]/miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/[folder of your choice]/miniconda3/miniconda.sh
bash ~/[folder of your choice]/miniconda3/miniconda.sh -b -u -p ~/[folder of your choice]/miniconda3
rm -rf ~/[folder of your choice]/miniconda3/miniconda.sh

After installing, initialize your newly-installed Miniconda. The following commands initialize for bash and zsh shells:

~/{folder of your choice}/miniconda3/bin/conda init bash
~/{folder of your choice}/miniconda3/bin/conda init zsh

P.D. {folder of your choice}: it is where you want to download and install miniconda,
Ex. mkdir -p ~/[folder of your choice]/miniconda3 = mkdir -p ~/home/user/Downloads/miniconda3
