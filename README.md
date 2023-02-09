# Site selection protocol for the i-Trees project
As part of the i-Trees project a major data collection campaign will be started in 2023. Over the course of the summer the cooling effect of different tree species will be assessed in 8 different cities in the Netherlands.

There are tens of thousands of trees under municipal management in the respective cities. This poses the question of how to select the trees to be studied. Additional requirements for the selection are that trees in each city should be similarly situated. This prompts the need for a reproduceable approach for tree selection (hereafter the tree selection protocol).

The selection protocol uses different publicly accessible datasets, such as the national [Land Use dataset](https://www.nationaalgeoregister.nl/geonetwork/srv/eng/catalog.search#/metadata/6318009c-7b11-4ab9-9929-735584dfb692?tab=relations), the [national roads dataset](https://www.nationaalwegenbestand.nl/index.php/aanbieders) and the [3D BAG](https://3dbag.nl/en/viewer) developed by the [3D geoinformation group](https://3d.bk.tudelft.nl/) at TU Delft. Additionally, a dataset of trees was provided by the i-Tree project. 

Criteria selection is implemented as follows:

Trees in parks:

trees shall be at least x m away from other landuse
trees shall be isolated from other trees (free standing), which is assessed by calculating the crown cover % in a x m buffer around each tree.
trees shall be in a specific density environment which is assessed by calculating the Ground Space Index (a built up area density measure) in a x m buffer around it.
Trees in street canyons:

trees shall be located in streets that are oriented e-w (within a healthy margin) so building shadows don't interfere with the measurements.
trees shall be located in streets with a width >= x.
trees shall be located in streets with a h/w ratio of <= x.
trees shall be in a specific density environment which is assessed by calculating the Ground Space Index and Floor Space Index.

If not already done, please install all libraries and dependencies using the environment.txt file using:

$ conda create -n --file req.txt

The prerequesite data folder will be shared at a later point in the project. 

