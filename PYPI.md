Packaging Python Projects
=========================
Reference:
https://packaging.python.org/tutorials/packaging-projects/

Requirements
------------
`pip install setuptools wheel twine`


Generating distribution archives
--------------------------------
`python3 setup.py sdist bdist_wheel`


Uploading the distribution archives
-----------------------------------
`python3 -m twine upload --repository-url https://test.pypi.org/legacy/ dist/* -u teamqwl -p TeamL*2`

Once you've successfully uploaded to PyPI Test, perform the same steps but point to the live PyPI server instead.

`python3 -m twine upload dist/* -u teamqwl -p TeamL*2`

and you're done!
