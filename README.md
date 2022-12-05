# VideoCC

VideoCC is a dataset containing (video-URL, caption) pairs for training
video-text machine learning models. 

It is created using an automatic pipeline starting from the Conceptual Captions
Image-Captioning Dataset. 

![videocc-pipeline](assets/images/videocc_pipeline.png)
## Paper 

More details are available in [this
paper](https://arxiv.org/pdf/2204.00679.pdf) at ECCV 2022. Please cite the paper if
you use or discuss this dataset in your work.

<div class="highlight highlight-source-shell"><pre>
@inproceedings{nagrani2022learning,
  title = {Learning Audio Video Modalities from Image Captions},
  author = {Nagrani, Arsha and Hongsuck Seo, Paul and Seybold, Bryan, and Hauth Anja, and Santiago, Manen, and Chen, Sun and Schmid, Cordelia},
  booktitle = {ECCV},
  year = {2022},
}
</pre></div>

## Data Format for VideoCC 

The data is provided [here](https://storage.googleapis.com/videocc3m/video_cc_public.csv)(note the file should start downloading immediately) as a single CSV file with the following columns: 

Video URL, Start timestamp (microseconds), End timestamp(microseconds), Caption. 

The data will not be exactly the same as the dataset used to train models in the
paper but should be similar. Note that some sections of YouTube videos might contain static frames
that are panned in or out. These can be filtered out using a motion filtering
tool. 


