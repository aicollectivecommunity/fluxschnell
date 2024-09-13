<h1>Flux Schnell implementation with low mem </h1>
<p>First version: 12/09/2024</p>
<p>Author: Nicolas MARTIN</p>

<h2>Introduction</h2>
<p>This repository has been created to be used in any Virtual Machine, preferably in a cloud platform (ex: Vast.ai or Paperspace).</p>

<h2>Prerequisites</h2>


<ul>
<li>16 GPU VRAM</li>
<li>Docker</li>
<li>70GB disk memory</li>
</ul>

<h2>Step 1</h2>

<p>pull fractalapps/genimages:v0815a in to your Virtual Machine. </p>

<p>If the GPU cloud service doesn't have any predeined run command, use: </p>
<p>docker run -d -p 8888:8888 -e PIP_DISABLE_PIP_VERSION_CHECK=1 fractalapps/genimages:v0813a jupyter lab --allow-root --ip=0.0.0.0 --no-browser --ServerApp.trust_xheaders=True --ServerApp.disable_check_xsrf=False --ServerApp.allow_remote_access=True --ServerApp.allow_origin='*' --ServerApp.allow_credentials=True</p>

<h2>Step 2</h2>
<p>Run Flux_lowmem.ipynb on Jupyter Lab.</p>
