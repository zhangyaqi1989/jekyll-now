---
layout: post
title: Use Jupyter Notebook Remotely
---

Recently I starts to refresh my knowledge on deep learning. I have a desktop in the lab which 
has a GTX 1080 Ti GPU in it. I usually use my laptop to ssh onto it.
So it would be handy if I can use Jupyter Notebook remotely.
After googling a while, I found the [solution](https://amber-md.github.io/pytraj/latest/tutorials/remote_jupyter_notebook).


First of all, log to the remote machine and type below command in the terminal.

```bash
jupyter notebook --no-browser --port=8080
```

Then on your local machine, type below command in the terminal.

```bash
ssh -N -L localhost:8080:localhost:8080 username@remote_host_name
```

Now open your local browser and go to the below address

```bash
localhost:8080
```
