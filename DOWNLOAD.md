Dataset **CCP** can be downloaded in [Supervisely format](https://developer.supervisely.com/api-references/supervisely-annotation-json-format):

 [Download](https://assets.supervisely.com/supervisely-supervisely-assets-public/teams_storage/S/P/KZ/FFwOGQToXLuZf7Os6rBHGOt4k5POtLyc5Y6exNqNMoYfOoYeulcrdsr4TFFFo0T8VgZxMozKFxiw93TkCykHHg1Ma60UMKCJO0P1Tj9xxRj6IxvLeWt8DKLZih2E.tar)

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

