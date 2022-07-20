# geo4dev-ct-map

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Atlas AI Geo4Dev Crop Type Mapping Tutorial</span> by <span xmlns:cc="http://creativecommons.org/ns#" property="cc:attributionName">Atlas AI P.B.C. and the World Bank's Development Data Group</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

### Environment set-up

#### GEE account

- You will need to sign up to the [GEE platform](https://earthengine.google.com/) with a Google account. Google Earth Engine remains free of charge for academic institutions, so you can sign up for free with your berkeley.edu email. Google usually gives access to new users within 24 hours. 
- Data in GEE can be analyzed in two ways:
  - through the Javascript API via the GEE [code editor](https://code.earthengine.google.com/), or
  - through the [Python API](https://developers.google.com/earth-engine/tutorials/community/intro-to-python-api), that can be accessed through any Python environment, such as Jupyter notebooks. 

#### Python

- Make sure you have Python 3.7+ installed on your computer
  - Also install [conda](https://conda.io/en/latest/) for package management 
- Set up a different environment for this workshop - let’s call it `ct_map`. You can use conda to do that as follows:
  - `conda create --name ct_map python=3.7.10`
  - `conda activate ct_map`
- Install some requirements in your environment:
  - `conda install jupyter`
  - `conda install gdal`
  - `pip install git+https://github.com/shrutijain90/eetc.git@v0.0.10` 
    - If you are unable to install the `gee-tools` repo using the above command, try installing it in edit mode as follows:
      - Clone the repo: `git clone https://github.com/shrutijain90/eetc.git`
      - cd into the repo directory 
      - `pip install -e .`
  - `conda install pandas`
  - `conda install geopandas`
  - `conda install geemap -c conda-forge`
  - `conda install -c anaconda scikit-learn`
  - `pip install eeconvert`
  - `conda install -c anaconda seaborn`
- Authenticate earth engine 
  - `earthengine authenticate`
