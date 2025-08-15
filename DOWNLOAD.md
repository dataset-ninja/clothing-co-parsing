Dataset **CCP** can be downloaded in [Supervisely format](https://developer.supervisely.com/api-references/supervisely-annotation-json-format):

 [Download](https://assets.supervisely.com/remote/eyJsaW5rIjogInMzOi8vc3VwZXJ2aXNlbHktZGF0YXNldHMvMjQzOF9DQ1AvY2NwLURhdGFzZXROaW5qYS50YXIiLCAic2lnIjogInFMMmUxR0dmdmRuZThGS3UvVXVsL2U0R1ZoYTVFSjBrRUFORzdTN2tvOFk9In0=?response-content-disposition=attachment%3B%20filename%3D%22ccp-DatasetNinja.tar%22)

As an alternative, it can be downloaded with *dataset-tools* package:
``` bash
pip install --upgrade dataset-tools
```

... using following python code:
``` python
import dataset_tools as dtools

dtools.download(dataset='CCP', dst_dir='~/dataset-ninja/')
```
Make sure not to overlook the [python code example](https://developer.supervisely.com/getting-started/python-sdk-tutorials/iterate-over-a-local-project) available on the Supervisely Developer Portal. It will give you a clear idea of how to effortlessly work with the downloaded dataset.

