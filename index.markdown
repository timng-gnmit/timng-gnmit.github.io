---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Home
---
<h1 style="text-align: left;"> Hello! I'm Tim.
  <div id="image-div" style="float:right;">
    <!-- <span style="float:right;"> -->
      <img id="tim-pic" src="https://raw.githubusercontent.com/timng-gnmit/timng-gnmit/refs/heads/main/tim.png" alt="Timothy Ng" width="200" hspace="50"/>
    <!-- </span> -->
  </div>
</h1> 

I'm interested in mathematics, machine learning, and solving interesting problems. I most recently received my Master of Data Science at the University of California, Irvine in December 2025, and I acquired my Bachelor of Science in Mathematics from the University of California, Davis in June 2023.

If you're curious about what I've been up to, check out my <a href="./projects.html">projects</a> or my [GitHub profile](https://github.com/timng-gnmit). Thanks for coming by!

<h2 id="projects" style="text-align: left;">Project Highlights</h2>
- Soccer Analytics Dashboard ([git repo](https://github.com/TrilemmaFoundation/UCI-MDS-F25-Soccer), [dashboard](https://uci-mds-f25-soccer.streamlit.app/))
- Latent Dirichlet Allocation of the BBC News Archive ([git repo](https://github.com/timng-gnmit/CS275P-LDA))
- LDA and QDA vs Random Forests for classification of Optimal Soccer Positions ([slides](http://timng-gnmit.github.io/projects/FinalProjectSTAT240P_ChoiGaoNgSuradja.html))
<!--
| Project | Link |
|:-------|:----:|
| Latent Dirichlet Allocation of the BBC News Archive | [GitHub Repository](https://github.com/timng-gnmit/CS275P-LDA) |
| LDA and QDA vs Random Forests for classification of Optimal Soccer Positions | [Slides](http://timng-gnmit.github.io/projects/FinalProjectSTAT240P_ChoiGaoNgSuradja.html) |
-->
{% raw %}
<script>
  imgElementDiv = document.getElementById('image-div');
  imgElement = document.getElementById('tim-pic');
  // image width is 200 + 50 hspace on both sides = 300
  // text should get at least half the space so check if width is 600 or more?
  window.addEventListener('load', formatImage);
  window.onresize = formatImage;
  function formatImage() {
        const width = window.innerWidth;
    console.log(width);
    if (width > 500) {
      // console.log("hi I'm here");
      imgElementDiv.style = "float:right;";
      imgElement.hspace = 50;
      imgElement.width = 200;
    } else {
      // console.log("still here");
      imgElementDiv.style = "float:none;";
      imgElement.hspace = 0;
      imgElement.width = Math.max(width, 200);
    }
  }
</script>
{% endraw %}