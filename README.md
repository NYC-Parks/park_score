## About the Project
The Park Condition Score (PCS) is a comprehensive score ranging from 0 to 100, derived from a vast amount of highly vetted underlying Parks Inspection Program (PIP) data. This score serves as a broad indicator and offers insight into the overall condition of your neighborhood park. It encompasses various aspects, including cleanliness metrics such as litter, structural elements such as play equipment, landscape features such as lawns and trees, and the state of amenities within restrooms.

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



## Getting Started

#### Create a conda environment from the yml file

```
conda env create --name YOURENVNAME --file park_score.yml
```

#### Activate the environment
```
conda activate YOURENVNAME
```

#### Add a kernel for your environment
```
python -m ipykernel install --user --name=YOURENVNAME
```

#### Run the Jupyter notebook
```
jupyter notebook
```

#### Set the kernel YOURENVNAME. Below, the kernel is set to park_score_public.
![Select Kernel](media/SelectKernel.jpg)


#### Enjoy!

-----------------------------------------------------------

#### To deactivate your environment
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

