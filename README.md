# python-lib-2-pkg
A json-file with mappings between python library names and python package names

## Format of JSON file
```bash
{
  [PYTHON_LIBRARY_NAME]: 
  {
    "package_names": [
        {
                    "date_added": [yyyy-mm-dd],
                    "downloads": [DOWNLOAD_COUNTS_FROM_PYPI],
                    "package_name": [PACKAGE_NAME]
                }
            ]
        },
        ...
      ]

  }
}
```

**[PYTHON_LIBRARY_NAME]**: is the name of a python library as seen in:
```python
import numpy            # library name: numpy 
from PIL import Image   # library name: PIL 
```

**[PACKAGE_NAME]**: is the corresponding python package names as found on PyPi, which can be installed through e.g. pip to be able to import the python library. Examples: 
```bash
pip install opencv-python
```
to be able to import cv2 and:
```bash
pip install scikit-learn
```
to be able to import sklearn

