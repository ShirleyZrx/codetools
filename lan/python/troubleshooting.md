## problems and solutioins
### error: subprocess-exited-with-error
```
Obtaining file:///home/${username}/sensecore/opencompass/opencompass
  Preparing metadata (setup.py) ... error
  error: subprocess-exited-with-error

  × python setup.py egg_info did not run successfully.
  │ exit code: 1
  ╰─> [100 lines of output]
      /home/${username}/anaconda3/envs/opencompass/lib/python3.10/site-packages/setuptools/__init__.py:88: _DeprecatedInstaller: setuptools.installer and fetch_build_eggs are deprecated.

Solution:
pip install --upgrade setuptools
```

### ERROR: launchpadlib 1.10.13 requires testresources, which is not installed.
```
ERROR: launchpadlib 1.10.13 requires testresources, which is not installed.

Solution:
pip install testresources
tips: use pip with the correct version
```

### urllib3.exceptions.ReadTimeoutError: HTTPSConnectionPool(host='files.pythonhosted.org', port=443): Read timed out.
```
urllib3.exceptions.ReadTimeoutError: HTTPSConnectionPool(host='files.pythonhosted.org', port=443): Read timed out.

Solution:
~$ python3 -m pip install --upgrade pip -i https://pypi.tuna.tsinghua.edu.cn/simple/
```

### error: subprocess-exited-with-error
```
  error: subprocess-exited-with-error

  × python setup.py egg_info did not run successfully.

Solution:
pip install --upgrade pip setuptools==57.5.0 -i https://pypi.tuna.tsinghua.edu.cn/simple/
```
