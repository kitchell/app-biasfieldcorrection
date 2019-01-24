[![Abcdspec-compliant](https://img.shields.io/badge/ABCD_Spec-v1.1-green.svg)](https://github.com/brain-life/abcd-spec)
[![Run on Brainlife.io](https://img.shields.io/badge/Brainlife-bl.app.14-blue.svg)](https://doi.org/10.25663/bl.app.14)

# app-biafieldcorrection
This service corrects the bias field of T1 and DWI images using ANTs

### Author
- Lindsey Kitchell (kitchell@indiana.edu)

### Funding 
[![NSF-BCS-1734853](https://img.shields.io/badge/NSF_BCS-1734853-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1734853)
[![NSF-BCS-1636893](https://img.shields.io/badge/NSF_BCS-1636893-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1636893)

## Running the App 

### On Brainlife.io

You can submit this App online at [https://brainlife.io/app/5a0f2dba19b13d1e190f1eeb#](https://brainlife.io/app/5a0f2dba19b13d1e190f1eeb#)  and [https://brainlife.io/app/5ae9c55df446980028b15eba#](https://brainlife.io/app/5ae9c55df446980028b15eba#) via the "Execute" tab.

### Running Locally (on your machine)

1. git clone this repo.
2. Inside the cloned directory, create `config.json` with something like the following content with paths to your input files.

```json
{
    "t1": ../ti.nii.gz
}
```
3. Execute the main file via command line

### Sample Datasets

If you don't have your own input file, you can download sample datasets from Brainlife.io, or you can use [Brainlife CLI](https://github.com/brain-life/cli).


## Output

The main output of this App is the bias corrected image (t1 or dwi) and the bia.nii.gz field image. 


### Dependencies

This App require ANTs to run. ANTs can be obtained from [http://stnava.github.io/ANTs/](http://stnava.github.io/ANTs/).
