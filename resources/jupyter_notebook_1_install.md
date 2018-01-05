# Jupyter Notebook:  Getting Started
The Jupyter notebook is an interactive computational environment, in which you can combine code, execution, rich text, mathematics, plots and rich media. 

---

### [Install the Notebook](http://jupyter.readthedocs.io/en/latest/install.html)
Installing Jupyter using Anaconda and conda:  
For new users, we highly recommend [installing Anaconda](https://www.continuum.io/downloads). Anaconda conveniently installs Python, the Jupyter Notebook, and other commonly used packages for scientific computing and data science.  (Prereq: Python is installed.)

Once anaconda is installed, you can launch the notebook by typing
```{bash}
$ jupyter notebook
```

### Upgrade all libraries/packages
We will now update all the packages/libraries installed by anaconda to ensure you have the latest version of everything!

```{bash}
$ conda update --all
```

### Run the Notebook at Terminal Prompt  
Note:  The notebook will open at the directory in which you launch the notebook on your terminal.  
```
$ jupyter notebook
```
```console
Adafoo:~ bugclimber$ jupyter notebook
[I 13:40:21.446 NotebookApp] Serving notebooks from local directory: /Users/bugclimber
[I 13:40:21.446 NotebookApp] 0 active kernels 
[I 13:40:21.446 NotebookApp] The Jupyter Notebook is running at: http://localhost:8888/?token=44cff804f386579f172ca44e41585c3b12749024c3c3bcda
[I 13:40:21.446 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
[C 13:40:21.447 NotebookApp] 
    
    Copy/paste this URL into your browser when you connect for the first time,
    to login with a token:
        http://localhost:8888/?token=44cff804f386579f172ca44e41585c3b12749024c3c3bcda
[I 13:40:21.556 NotebookApp] Accepting one-time-token-authenticated connection from ::1
```

```console
reshama$ jupyter notebook
[I 11:41:22.769 NotebookApp] Serving notebooks from local directory: /Users/reshamashaikh/_ds/metis
[I 11:41:22.769 NotebookApp] 0 active kernels 
[I 11:41:22.769 NotebookApp] The Jupyter Notebook is running at: http://localhost:8888/
[I 11:41:22.769 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
```

### Shut Down the Juypter Notebook App
At terminal prompt:  
 * control + c
 * type:  `y`
 
```console
^C[I 13:43:34.900 NotebookApp] interrupted
Serving notebooks from local directory: /Users/bugclimber
0 active kernels 
The Jupyter Notebook is running at: http://localhost:8888/?token=44cff804f386579f172ca44e41585c3b12749024c3c3bcda
Shutdown this notebook server (y/[n])? y
[C 13:43:36.548 NotebookApp] Shutdown confirmed
[I 13:43:36.549 NotebookApp] Shutting down kernels
```

```console
^C[I 11:43:35.486 NotebookApp] interrupted
Serving notebooks from local directory: /Users/reshamashaikh/_ds/metis
0 active kernels 
The Jupyter Notebook is running at: http://localhost:8888/
Shutdown this notebook server (y/[n])? y
[C 11:43:37.782 NotebookApp] Shutdown confirmed
[I 11:43:37.783 NotebookApp] Shutting down kernels
reshama$ 
```

---

### Getting to Know Jupyter

You can try out Jupyter on a browser without installing it.  
https://try.jupyter.org/

