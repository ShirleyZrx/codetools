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

### ERROR: Ignored the following versions that require a different python version: 1.25.0
```
INFO: pip is looking at multiple versions of opencompass to determine which version is compatible with other requirements. This could take a while.
ERROR: Ignored the following versions that require a different python version: 1.25.0 Requires-Python >=3.9; 1.25.1 Requires-Python >=3.9; 1.25.2 Requires-Python >=3.9; 1.26.0 Requires-Python <3.13,>=3.9; 1.26.1 Requires-Python <3.13,>=3.9; 1.26.2 Requires-Python >=3.9; 1.26.3 Requires-Python >=3.9; 1.26.4 Requires-Python >=3.9; 1.4.0 Requires-Python >=3.9; 1.4.0rc1 Requires-Python >=3.9; 1.4.1.post1 Requires-Python >=3.9; 1.4.2 Requires-Python >=3.9; 1.5.0 Requires-Python >=3.9; 1.5.0rc1 Requires-Python >=3.9; 1.5.1 Requires-Python >=3.9; 1.5.2 Requires-Python >=3.9; 2.0.0 Requires-Python >=3.9; 2.0.1 Requires-Python >=3.9; 2.0.2 Requires-Python >=3.9; 2.1.0 Requires-Python >=3.10; 2.1.0 Requires-Python >=3.9; 2.1.0rc0 Requires-Python >=3.9; 2.1.0rc1 Requires-Python >=3.10; 2.1.1 Requires-Python >=3.10; 2.1.1 Requires-Python >=3.9; 2.1.2 Requires-Python >=3.9; 2.1.3 Requires-Python >=3.9; 2.1.4 Requires-Python >=3.9; 2.2.0 Requires-Python >=3.9; 2.2.0rc0 Requires-Python >=3.9; 2.2.1 Requires-Python >=3.9; 2.2.2 Requires-Python >=3.9
ERROR: Could not find a version that satisfies the requirement scikit_learn==1.5.0 (from opencompass) (from versions: 0.9, 0.10, 0.11, 0.12, 0.12.1, 0.13, 0.13.1, 0.14, 0.14.1, 0.15.0, 0.15.1, 0.15.2, 0.16.0, 0.16.1, 0.17, 0.17.1, 0.18, 0.18.1, 0.18.2, 0.19.0, 0.19.1, 0.19.2, 0.20.0, 0.20.1, 0.20.2, 0.20.3, 0.20.4, 0.21.1, 0.21.2, 0.21.3, 0.22, 0.22.1, 0.22.2, 0.22.2.post1, 0.23.0, 0.23.1, 0.23.2, 0.24.0, 0.24.1, 0.24.2, 1.0, 1.0.1, 1.0.2, 1.1.0, 1.1.1, 1.1.2, 1.1.3, 1.2.0rc1, 1.2.0, 1.2.1, 1.2.2, 1.3.0rc1, 1.3.0, 1.3.1, 1.3.2)
ERROR: No matching distribution found for scikit_learn==1.5.0


Solution:
conda activate opencompass
```
