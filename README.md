### Python Results Uploader

This repository creates a docker container that you can upload your results to it. So you can implement your own distributional results uploader.


Usage:

```python
# In your own python file

REMOTE_ROOT = "/root/Counterfactual_IRS"
LOCAL_PATH = logger_path # it is a related path, e.g., "./mypath/mylog.log"
REMOTE_PATH = os.path.join(REMOTE_ROOT, os.path.dirname(LOCAL_PATH)) # E.g., "/root/Counterfactual_IRS/./mypath/mylog.log"

my_upload(LOCAL_PATH, REMOTE_PATH, REMOTE_ROOT)
```

