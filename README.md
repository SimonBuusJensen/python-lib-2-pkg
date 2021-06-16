# python-lib-2-pkg
A json-file with mappings between python library names and python package names

## Format of JSON file
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

[PYTHON_LIBRARY_NAME]: is the name of a python library as seen in "import **numpy**" or "from **PIL** import Image" (e.g. numpy and PIL)

[PACKAGE_NAME]: is the corresponding python package name as found on PyPi. Examples: **opencv-python**, **scikit-learn**

