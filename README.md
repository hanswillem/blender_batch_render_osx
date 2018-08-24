# Blender Batch Render

#### Put multiple .blend files in a render queue and render them in one go as a background job. It's also possible to render different renderlayers as seperate image sequences.

### Install instructions

Install Blender in the **default location** *(C:/Program Files/Blender Foundation/Blender/blender.exe)*. Download *add-on_batch_render_windows.py* and copy it to a folder. Look for the following line in the file  and edit it so that it points to that folder.
```python
batch_file = 'P:/_blender_batch_render/batch_render.bat'
```
Start Blender and install *add-on_batch_render_windows.py* as a Blender Add-on. A new tab called *Batch Render* should show up in the Tools region (toggled on and off with the shortcut 't'). 

### Basic Usage

The Add-on is pretty straightforward. You can add .blend files to the queue, and clear the queue. You can't start rendering from the Add-on directly because Blender would freeze until all the files are rendered. Instead, click on *Open Folder* and then double click on *batch_render.command*. Blender then starts rendering all the files in the queue as a background job.  

#### Add layers To Queue You

When this button is clicked, every renderlayer of the open file is added to the queue as a seperate file. This makes it possible to render every renderlayer as a seperate image sequence.
