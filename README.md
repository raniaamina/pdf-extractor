# PDF Extractor

Simple script to help extracting PDF file and/or convert them to SVG. This script created in order to help them who need import multiple pdf page easily in to inkscape.

## Dependencies
- pdftk
- inkscape
- ghostscript

For Ubuntu 18.04 user or older, maybe you can't find install dependency via apt. You can install it via snap or add ppa:malteworld/ppa. Second option is best choice for WSL user. 

```
sudo add-apt-repository ppa:malteworld/ppa
sudo apt update
sudo apt install pdftk
```

## Install
Make sure git installed on your system before running command bellow.

```bash
git clone https://github.com/raniaamina/pdf-extractor.git ~/.config/pdf-extractor
cd ~/.config/pdf-extractor
sudo chmod +x pdf-extractor
sudo ln -s ~/.config/pdf-extractor/pdf-extractor /usr/local/bin/pdf-extractor
```

## Usage
basic usage:
`pdf-extractor file-name.pdf`

**Example step:**
1. Open your terminal
2. Go to directory where multiple page pdf saved. For example, if your pdf document saved in my-document folder in home, you can type `cd ~/my-document`. 
3. `pdf-extractor file-name.pdf`
4. Now, you can choose one of actions that provided.

Type: `pdf-extractor --help` for more information


## Known Problem
Some of distribution can't use/get pdftk from PPA, so here is an option if you get a problem with installing pdftk.
1. sudo apt install default-jre-headless libcommons-lang3-java libbcprov-java
2. download the deb file of pdftk-java from https://packages.ubuntu.com/focal/pdftk-java
3. download the deb file of pdftk from https://packages.ubuntu.com/focal/pdftk

Thanks for (@alezzacreative)[https://github.com/alezzacreative] who giving information about this.



## Disclaimer
This script basicly only structured command that arranged to made it easy to use for specific purpose. PDF Extractor come with no warranty, so use with your own risk. 

[Rania Amina](https://raniaamina.id)
