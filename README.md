# practice-DocumentationCPPPython
Project to practice documentation for C++ and Python

This project is based on the documentation available at:  
https://devblogs.microsoft.com/cppblog/clear-functional-c-documentation-with-sphinx-breathe-doxygen-cmake/

## Getting Started

Clone or download the project.  
Recommended: Create a virtual environment and install the sphinx package.  
python -m venv env  

Windows:  
env\Source\activate.bat  
Linux:  
source env\bin\activate  

### Prerequisites

Install Doxygen  
https://www.doxygen.nl/download.html  
Add to the environment path the location of the doxygen binary (i.e. C:/Program Files/Doxygen/bin).  
pip install -U Sphinx  
pip install sphinx-rtd-theme  
pip install breathe

### Installing

This project does not requires installation.  

## List of projects

* Empty :)  

## Running the tests

This project differs form the original documentation in how the folders are structured.  

### Break down into end to end tests

mk docs  
cd docs  
sphinx-quickstart  
modify conf.py  
  Uncomment/modify the following lines  
  import os
  import sys
  sys.path.insert(0, os.path.abspath('../src'))

To autogenerate the rst files, run the sphinx-apidoc command using the following syntax:  
sphinx-apidoc -o <OUTPUT_PATH> <MODULE_PATH>  
In our example, the output directory is source , and the module directory is src.  
sphinx-apidoc -f -o source ..\src  

modify index.rst  

  add source/modules  

modify the other rst files...  

## Contributing

All contributions are welcome :).

## Versioning

The project uses semantic versioning.  
https://semver.org/  
Version 0.1.0  

## Authors

* **Khoronus** - *Initial work* - [Khoronus](https://github.com/Khoronus)

## License

This project is licensed under (see the [LICENSE.md](LICENSE.md) file for details).

## Acknowledgments

* Empty :)


## Resources  

https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html  
https://google.github.io/styleguide/pyguide.html  