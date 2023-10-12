---
layout: default
---

<span class="sys-name">🔮 GenQuery</span> is an <span class="highlight">interactive visual search system</span> that allows the users to concretize the abstract text query <span class="highlight">[a]</span>, express search intent through visuals <span class="highlight">[b]</span>, and diversify their search intent based on the search history <span class="highlight">[c]</span>. Through the three main features, users can express their visual search intent easily and accurately and explore a more diverse and creative visual search space.
<br/>

{: .sys-img}
![Three main features of GenQuery: (1) Query concretization, (2) Image-based image modification, and (3) Keyword-based image modification feature. Query concretization concretizes the user's vague text query for the text-based search. Image-based image modification allows the user to select the area in an image (red dot line above) and to change the area of the image based on the reference image (purple mountain image). Keyword-based modification allows the user to change the selected area of an image (red dot line below) based on the keywords suggested from the user's search history. Both modification features' output could be utilized as an image-based search input and the results are changed due to the image modifications.](/assets/img/teaser.png)

---

## <span class="sys-name">Interface</span>

{: .sys-img}
![Interface of GenQuery. GenQuery shows the image search results as a gallery form. (a) Text prompt input box for text-based search: User can input a text description for the desired image here; (b) Clickable image for image-based search: An image in the gallery is clickable to provoke the image-based search. When the image is clicked, GenQuery shows similar images to the clicked one at the bottom of the gallery; (c) Like button: The user can click the like button to save the design into the side panel; (d) Generation button: To edit one of the searched images for generatin a new input, the user can click the marble emoji left top of image card. When the user clicks this button, the generation panel pops out below; (e) Show more button: This button is clicked when the user wants to see more search results.](/assets/img/interface.png)

<span class="sys-name">🔮 GenQuery</span> provides a similar interface to popular visual search tools like [Pinterest](https://co.pinterest.com/). The system provides a similar interface to popular visual search tools like Pinterest. Users can input a text query <span class="highlight">[a]</span> (text-based search) or click an image in the search results <span class="highlight">[b]</span> (image-based search) to find the visual images they want to see and save the desired images <span class="highlight">[c]</span>.

Beyond these basic features, <span class="sys-name">GenQuery</span> supports **<a href="#QC" target="_self">Query Concretization</a>** when the user writes a query in <span class="highlight">[a]</span>. Furthermore, when the user clicks <span class="highlight">[d]</span>, it also supports **<a href="#IM" target="_self">Image-based Image Modification</a>** and **<a href="#KM" target="_self">Keyword-based Image Modification</a>** to allow the user to find more intent-aligned or diversified images.

<br/>

### <span id="QC" class="sys-name">Query Concretization</span> for Text-based Search

Our formative study findings reveal that the visual search process is inefficient due to the user's vague text query at the initial text-based search. To address this, we propose a <span class="sys-name">Query Concretization</span> interaction using LLM prompting in the visual search process.

<div class="video-wrapper">
  <iframe src="https://www.youtube.com/embed/8AhXwrU3WS4?si=tdU7Q55_YXL3ChDY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

<br/>

### <span id="IM" class="sys-name">Image-based Image Modification</span> for Image-based Search

When users had concrete target images they wanted to look for in their minds, they wanted to use image modality to edit the following search queries in the image-based search. To support the user in finding a more intent-aligned search result, we propose <span class="sys-name">Image-based Image Modification</span> for the following visual search query.

<div class="video-wrapper">
  <iframe src="https://www.youtube.com/embed/N-F3DsbE1fI?si=-7gaKdnObBQ1g-jH" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

<br/>

### <span id="KM" class="sys-name">Keyword-based Image Modification</span> for Image-based Search

One of the essential aspects of visual search is finding diversified and unexpected ideas as well as searching intent-aligned images. Our formative findings identified that the users tried to use text modality when they wanted to see more diversified and different images. Thus, we propose <span class="sys-name">Text-based Image Modification</span> interaction to help the divergent visual search phase.

<div class="video-wrapper">
  <iframe src="https://www.youtube.com/embed/zJTqnCh8d2w?si=-vIMSjUHxgH-o6I_" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

---

The three interactions of <span class="sys-name">🔮 GenQuery</span> allowed the user to express their intent intuitively and accurately so that the users find more satisfied, diversified, and creative ideas. If you want to see more details of the findings of our user study, please check our paper!

## Bibtex

<pre>
@inproceedings{son2023genquery,
      title={GenQuery: Supporting Expressive Visual Search with Generative Models}, 
      author={Kihoon Son and DaEun Choi and Tae Soo Kim and Young-Ho Kim and Juho Kim},
      year={2023},
      eprint={2310.01287},
      archivePrefix={arXiv},
      primaryClass={cs.HC}
}
</pre>

---

{: .logos}
[![Logo of KIXLAB](/assets/img/kixlab_logo.png)](https://kixlab.org)
[![Logo of KAIST](/assets/img/kaist_logo.png)](https://kaist.ac.kr)
[![Logo of NAVER](/assets/img/naver_logo.png)](https://www.facebook.com/NAVERAILAB)

{: .center .acknowledgement}
This research was supported by the **KAIST-NAVER Hypercreative AI Center**.
