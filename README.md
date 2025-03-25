## About the Project
The Park Condition Score (PCS) is a comprehensive score ranging from 0 to 100, derived from a vast amount of highly vetted underlying Parks Inspection Program (PIP) data. This score serves as a broad indicator and offers insight into the overall condition of your neighborhood park. It encompasses various aspects, including cleanliness metrics such as litter, structural elements such as play equipment, landscape features such as lawns and trees, and the state of amenities within restrooms.

The Park Condition Score represents a 3-year rolling average with a 2-month lag. This means that the score reflects data from 3 years and 2 months prior to today's date. The scores displayed on the Parks website are updated daily at 4:00 AM.


## How It's Calculated
The score evaluates seventeen distinct features across three categories: Cleanliness, Structural and Landscape. Cleanliness carries the greatest weight, accounting for 50% of the PCS, followed by Structural at 30% and Landscape at 20%. 

Each feature in these categories is rated as Pass (A), Not Rated (N), Unacceptable (U), or Unacceptable for Site (U/S). When an aspect is rated as U or U/S, deductions are applied to the PCS.  The weights for each aspect vary within their respective categories; for instance, litter and restroom litter heavily influence the Cleanliness category, play equipment and paved surface heavily impact the Structural scores, and lawns and trees heavily affect the Landscape category. 

The distinction between a U and U/S deduction is a magnitude of 3. When features receive a Not Rated (N), deductions are normalized. For example, if restrooms are absent from the site, penalties for other Cleanliness feature are adjusted accordingly.  

Below is an example of weights for a park that includes restrooms and all features within Structural and Landscape categories (Note: PR = Public Restroom):

<div align="center">
  
| Cleanliness (50%)    | Structural (30%) |  Landscape (20%)
| :--------: | :-------: | :--------: |
| litter 30%  | play equipment 25%    |  lawns 40% |
| PR litter 25% | paved surface 25%     | trees 25% |
| glass 15%    | safety surface 15%    |  athletic fields 20% |
| PR amenities 15% | benches 15% | horticultural areas 5% | 
| PR graffiti 5% | sidewalks 10% | trails 5% | 
| graffiti 5% | fences 5% | water bodies 5% | 
| ice/weeds 5% | PR structural 5% |    |

</div>



## Project Setup Guide

This project assumes you have [Anaconda](https://www.anaconda.com/docs/getting-started/anaconda/install), [Jupyter](https://anaconda.org/anaconda/jupyter), and [Git](https://git-scm.com/downloads) installed. 

## One-Time Setup (Initial Installation)

These steps are only required once to set up the environment.

### 1. Clone the Repository

To clone the repository, run the following command in your **Git Bash**:
```
git clone https://github.com/NYC-Parks/park_score.git
```

### 2. Create the conda environment

> [!NOTE]
> The following steps will take place in **Anaconda Prompt**.

To create the conda environment from the yml file to a specified path, open **Anaconda Prompt** and run the following command:
```
conda env create --name YOURENVNAME --file park_score.yml
```

To create the conda environment from file to a name (it will install the environment in the default location), run the following command:
```
conda env create -f E:\path\to\envName.yml --name YOURENVNAME
```

### 3. Install a kernel for Jupyter notebook for your new environment

To install ipykernel (just once), run: 
```
conda install ipykernel
```

To create new environment kernel for jupyter notebook, run: 
```
ipython kernel install --name=YOURENVNAME
```

For more information about jupyter notebooks and kernels, visit [this link](https://towardsdatascience.com/get-your-conda-environment-to-show-in-jupyter-notebooks-the-easy-way-17010b76e874/).


## Usage (After Setup is Complete)

Once installed, follow these steps each time you run the project.

### 1. Activate your environment
```
conda activate YOURENVNAME
```

#### Run the Jupyter notebook
```
jupyter notebook
```

#### Set the kernel YOURENVNAME. Below, the kernel is set to park_score_public.
![Select Kernel](media/SelectKernel.jpg)


## After usage

### 1. Deactivate your environment

```
conda deactivate YOURENVNAME
```

## Contributors
<table>
  <tbody>
    <td align="center" valign="top" width="14.28%"><a href="http://github.com/lilianchin6"><img src="media/LilianIcon.png" width="90px;"  alt="Lilian Chin"/><br /><sub><b>Lilian Chin</b></sub></a><br /></td>
    <td align="center" valign="top" width="14.28%"><a href="https://github.com/amaucoin"><img src="media/ArthurIcon.jpg" width="90px;" height="90px;" alt="Arthur Aucoin"/><br /><sub><b>Arthur Aucoin</b></sub></a><br /></td>
  </tbody>
</table>

