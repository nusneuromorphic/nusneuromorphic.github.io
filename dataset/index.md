<!--
.. title: Dataset
.. slug: dataset
.. date: 2021-02-05 10:59:23 UTC+08:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

The dataset is divided by event and RGB data recorded by the Inivation DAVIS240C camera and the ZED Stereo camera, respectively.

The event data is composed of binary files. To read them, the MATLAB AER Vision Functions are needed 
[https://github.com/gorchard/Matlab_AER_vision_functions](https://github.com/gorchard/Matlab_AER_vision_functions).

<ul>
    <li>Add the AER vision functions to the MATLAB path.</li>
    <li>Load a file using the "read_linux" function.<br> e.g. td = read_linux('../EBBINNOT/DAVIS_Events/Recording/20180711_Site1_3pm_12mm_01.bin'); </li>
    <li>Visualize the data using the ShowTD function.e.g. ShowTD(td);</li>
</ul>


Scripts to read the dataset and extract tracks from the annotation files are also included:
>For event data: make_dataset_images_full.m<br>
>For RGB data: make_dataset_images_RGB_full.m

The dataset is hosted in Zenodo [https://zenodo.org/record/3839231](https://zenodo.org/record/3839231).

Download links:
<br><a href="https://zenodo.org/record/3839231/files/EBBINNOT.zip?download=1">EBBINNOT Dataset</a>
<br><a href="https://zenodo.org/record/3839231/files/make_dataset_images_full.m?download=1">Extract events script</a>               
<a href="https://zenodo.org/record/3839231/files/make_dataset_images_RGB_full.m?download=1">Extract RGB script</a>

<h1>Samples:</h1>
<table style="width:70%">
  <tr>
    <td align=left><img src="/images/Dataset/event_Ebbinnot.jpg" width="500"/></td> 
    <td align=right><img src="/images/Dataset/frame2256.jpg"  width="500"/></td>
  </tr>
</table>
<br />  

<h1>License</h1>
This datasets are released under the [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/legalcode), which is free for non-commercial use (including research).
