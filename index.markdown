---
layout: default
---

<span class="sys-name">🔮 GenQuery</span> is an <span class="highlight">interactive visual search system</span> that allows the users to concretize the abstract text query <span class="sys-name">[a]</span>, express search intent through visuals <span class="sys-name">[b]</span>, and diversify their search intent based on the search history <span class="sys-name">[c]</span>. Through the three main features, users can express their visual search intent easily and accurately and explore a more diverse and creative visual search space.
<br/>

{: .sys-img}
![Three main features of GenQuery: (1) Query concretization, (2) Image-based image modification, and (3) Keyword-based image modification feature. Query concretization concretizes the user's vague text query for the text-based search. Image-based image modification allows the user to select the area in an image (red dot line above) and to change the area of the image based on the reference image (purple mountain image). Keyword-based modification allows the user to change the selected area of an image (red dot line below) based on the keywords suggested from the user's search history. Both modification features' output could be utilized as an image-based search input and the results are changed due to the image modifications.](/assets/img/teaser.png)

---

## <span class="sys-name">GenQuery Interface

The main screen of the interface consists of three panels.

{: .sys-img}
![Main screen of EvalLM shows three panels. The generation panel shows text boxes for the prompt and task instruction, and buttons for input sampling. The evaluation panel shows text boxes for the criteria, buttons for evaluating, and stacked bar charts for the evaluation results.](/assets/img/interface.png)

<b>Generation Panel</b>: To generate outputs, the user defines their overall **task instruction** (A), two **prompts** they want to compare (B), and then **samples inputs** from a dataset (C) which will be used to test the prompts.

**Evaluation Panel**: To evaluate outputs, the user defines a set of evaluation **<a href="#criteria" target="_self">criteria</a>** (D). Then, after evaluating, they can verify the overall _evaluation_ performance of each prompt (E) or, if they created a validation set, _validate_ how automatic evaluations align with ground-truth evaluations (F).

**Data Panel**: This panel shows **<a href="#datarow" target="_self">data rows</a>** containing inputs, outputs, and evaluation results.

<br/>

### <span id="criteria">Criteria</span>

{: .text-left}
<span class="sys-name">EvalLM</span> allows users to evaluate outputs on their own criteria specific to their application and/or context.
<br/><br/>
To define a criteria, the user simply provides the criteria with a **name** (A) and **description** (B) in natural language.
<br/><br/>
To assist users in creating more effective and helpful criteria, the system automatically **reviews** their criteria (C) and provides **suggestions** (D) on how the criteria can be _refined_, _merged_ and _split_.

{: .img-right}
![Criteria are represented as a set of text boxes that contain the name and description of the criteria. Suggested revisions are shown below the criteria.](/assets/img/criteria.png)

<br/>

### <span id="datarow">Data Row</span>

{: .sys-img}
![Data Rows in the interface display inputs, output pairs, and evaluation results. Clicking on evaluation results opens a panel that shows the explanation for that evaluation underneath the row.](/assets/img/datarow.png)

For each sampled **input** (A), the interface presents the **outputs** generated from each prompt side-by-side (B) and the **evaluation results** for each criteria next to the outputs (C). For each criteria, the evaluation results show which prompt produced the output that better satisfied that criteria.

If the user wants to see more details, they can click on one of these evaluations to see the assistant's **explanation** (D). To help the user match the explanation and outputs, the system also **highlights** spans from the outputs that were considered to be important when evaluating the criteria (E).

If the user selected to evaluate outputs on multiple trials, they can see the evaluations for **other trials** through the carousel (F).

---

## Video Demo

See <span class="sys-name">EvalLM</span> in action in this Video Demo.

{% if site.video %}

<div class="video-wrapper">
  <iframe src="{{site.video}}&color=white&rel=0&modestlogo=1" id="yt-video" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
{% endif %}

---

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
