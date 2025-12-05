---
layout: default
title: "Mohan Elapolu"
nav_exclude: true
---

<style>
  body {
    scroll-behavior: smooth;
    font-family: sans-serif;
    line-height: 1.55;
  }

  /* Each major section */
  section {
    padding: 25px 0;          /* increased vertical rhythm */
    border-bottom: 1px solid #eee;
    scroll-margin-top: 90px;  /* avoids sticky header overlap */
  }

  /* Section titles */
  h2 {
    margin-top: 0;
    margin-bottom: 12px;
    font-size: 26px;
    font-weight: 600;
  }

  </style>


<!-- EVERYTHING BELOW IS CENTERED -->
<div class="page-container">

<!-- Posts Section -->
<section id="home" markdown="1">
## Latest Posts

{% for post in site.posts limit:5 %}
- [{{ post.date | date: "%B %d, %Y" }}: {{ post.title }}]({{ post.url | relative_url }}) 
{% endfor %}

[View all posts →](/posts/)
</section>

<!-- ABOUT SECTION -->
<section id="about">

<div style="display:flex; justify-content:space-between; align-items:flex-start; gap:30px;">

  <!-- LEFT SIDE: MARKDOWN TEXT -->
  <div style="flex:1;" markdown="1">

## About Me

I am **Mohan Elapolu**, a computational scientist with a deep passion for understanding and predicting physical, chemical, biological, and engineered phenomena. 

I solve ODE/PDE-based systems using classical numerical methods and modern machine learning tools to build high- and low-fidelity simulations for complex system behavior, design optimization, and intelligent decision-making.

I construct advanced computational tools, including finite element solvers, finite-difference molecular dynamics frameworks, and physics-guided scientific machine learning models designed to run efficiently on high-performance computing environments. 

I also bring deep expertise in the modern Python and AI/ML stack—including GNNs, Transformers, generative AI (LLMs, RAG, agents), and MLOps practices for scalable deployment and workflow optimization.

I specialize in pre- and post-processing large-scale computational data using Python and scientific computing libraries to extract actionable insights and support data-driven reasoning.

  </div>

  <!-- RIGHT SIDE: PHOTO + ICONS -->
  <div style="width:230px; text-align:center; align-self:center;">


  <!-- PHOTO -->
  <img src="/assets/mohan.jpg" 
         alt="Mohan Elapolu" 
         style="width:200px; border-radius:12px; margin-bottom:12px;">

  <!-- ICONS -->
  <div style="display:flex; gap:20px; justify-content:center; align-items:center;>

  <!-- LINKEDIN -->
  <a href="https://www.linkedin.com/in/mohansuryarajaelapolu/" target="_blank">
    <svg width="26" height="26" viewBox="0 0 24 24" fill="#0077B5" xmlns="http://www.w3.org/2000/svg">
      <path d="M4.98 3.5C4.98 4.61 4.1 5.5 2.99 5.5C1.88 5.5 1 4.61 1 3.5C1 2.39 1.88 1.5 2.99 1.5C4.1 1.5 4.98 2.39 4.98 3.5ZM5 7H1V23H5V7ZM8.98 7H4.98V23H8.98V14.45C8.98 10.95 13.48 11.2 13.48 14.45V23H17.48V13.23C17.48 7.97 10.98 8.17 8.98 10.77V7Z"/>
    </svg>
  </a>

  <!-- GITHUB -->
  <a href="https://github.com/MohanElapolu" target="_blank">
    <svg width="26" height="26" viewBox="0 0 16 16" fill="black" xmlns="http://www.w3.org/2000/svg">
      <path d="M8 0C3.58 0 0 3.58 0 8C0 11.54 2.29 14.53 5.47 15.59C5.87 15.66 6.02 15.42 6.02 15.21C6.02 15.02 6.01 14.39 6.01 13.72C4 14.09 3.48 13.23 3.32 12.78C3.23 12.55 2.84 11.84 2.5 11.65C2.22 11.5 1.82 11.13 2.5 11.12C3.13 11.11 3.61 11.7 3.77 11.94C4.53 13.19 5.72 12.83 6.25 12.61C6.32 12.09 6.53 11.73 6.76 11.53C4.78 11.33 2.68 10.64 2.68 7.6C2.68 6.72 3 5.99 3.55 5.43C3.47 5.23 3.19 4.42 3.62 3.31C3.62 3.31 4.29 3.1 6.02 4.13C6.66 3.95 7.34 3.86 8.02 3.86C8.7 3.86 9.38 3.95 10.02 4.13C11.75 3.09 12.42 3.31 12.42 3.31C12.85 4.42 12.57 5.23 12.49 5.43C13.04 5.99 13.36 6.71 13.36 7.6C13.36 10.65 11.25 11.32 9.26 11.52C9.55 11.76 9.8 12.26 9.8 13.04C9.8 14.19 9.79 15.11 9.79 15.42C9.79 15.63 9.94 15.87 10.34 15.79C13.54 14.53 15.82 11.54 15.82 8C15.82 3.58 12.42 0 8 0Z"/>
    </svg>
  </a>

  <!-- GOOGLE SCHOLAR -->
  <a href="https://scholar.google.com/citations?user=79_RjssAAAAJ&hl=en" target="_blank">
    <svg width="26" height="26" viewBox="0 0 488 512" fill="#4285F4" xmlns="http://www.w3.org/2000/svg">
      <path d="M244 48L0 244L244 440L488 244L244 48ZM244 108L415 244L244 380L73 244L244 108Z"/>
    </svg>
  </a>

  <!-- RESUME -->
  <a href="/assets/resume.pdf" target="_blank">
    <svg width="26" height="26" viewBox="0 0 24 24" fill="#555" xmlns="http://www.w3.org/2000/svg">
      <path d="M14 2H6C4.9 2 4 2.9 4 4V20C4 21.1 4.9 22 6 22H18C19.1 22 20 21.1 20 20V8L14 2ZM13 9V3.5L18.5 9H13ZM8 12H16V14H8V12ZM8 16H14V18H8V16Z"/>
    </svg>
  </a>


  </div>
   <!-- ICONS -->
  <div style="display:flex; gap:20px; justify-content:center; align-items:center;>

  <!-- EMAIL -->
  <a href="mailto: mohanelapolu@gmail.com">
    <svg width="26" height="26" viewBox="0 0 24 24" fill="#D44638" xmlns="http://www.w3.org/2000/svg">
      <path d="M12 13L1 6.5V18C1 19.1 1.9 20 3 20H21C22.1 20 23 19.1 23 18V6.5L12 13ZM21 4H3C1.9 4 1 4.9 1 6L12 12L23 6C23 4.9 22.1 4 21 4Z"/>
    </svg>
  </a>

  <!-- TWITTER / X -->
  <a href="https://x.com/msrelapolu" target="_blank">
    <svg width="26" height="26" viewBox="0 0 24 24" fill="black" xmlns="http://www.w3.org/2000/svg">
      <path d="M18.244 2L12.63 9.14L6.36 2H2L10.39 11.23L2.32 22H6.82L12.76 14.52L18.57 22H22L13.48 12.27L21.18 2H18.244Z"/>
    </svg>
  </a>

  </div>

  </div>

</div>

</section>

<!-- RESEARCH SECTION -->
<section id="research">

<h2>Research</h2>

<style>
  .tabs-wrapper {
    margin-top: 20px;
  }

  .tab-row {
    display: flex;
    gap: 10px;
    border-bottom: 2px solid #ddd;
    padding-bottom: 5px;
  }

  .tab-row button {
    padding: 10px 20px;
    border: none;
    background: none;
    cursor: pointer;
    font-size: 16px;
    border-bottom: 3px solid transparent;
    transition: 0.2s;
  }

  .tab-row button.active {
    border-bottom-color: #0366d6;
    font-weight: bold;
    color: #0366d6;
  }

  .tab-content {
    display: none;
    margin-top: 20px;
  }

  .tab-content.active {
    display: block;
  }
</style>

<div class="tabs-wrapper">

<!-- HORIZONTAL TABS -->
<div class="tab-row">
  <button class="active" onclick="switchTab('t1', this)">Scientific ML</button>
  <button onclick="switchTab('t2', this)">Physics-based Predictive Analysis</button>
  <button onclick="switchTab('t3', this)">Systems Engineering</button>
</div>

<!-- TAB CONTENT SECTIONS -->
<div id="t1" class="tab-content active" markdown="1">

**FiGNNet: A Fracture-informed Graph Transformer-Attention Neural Network for Simulating Crack Propagation**

Modeling fracture in solids remains a significant challenge in computational mechanics due to the complexity of crack initiation and propagation under mixed-mode loading. In this work, we introduce a novel fracture-informed graph neural network (GNN) framework (FiGNNet) for simulating fractures in pre-cracked elastic solids. FiGNNet couples a graph transformer network (GTF) to capture long-range interactions with a graph attention network (GAT), focusing on localized behavior near crack tips. The governing equations of linear elasticity are embedded in the loss function through their weak form, ensuring physical consistency without relying on finite element analysis (FEA) solutions: displacements or stresses. The proposed approach is validated against FEA across various benchmark problems involving center and edge cracks subjected to tensile, shear, and bending loads. FiGNNet accurately predicts displacement fields, stress distributions, and crack propagation angles across all scenarios. The proposed method offers a physics-informed machine learning framework for fracture simulation, with strong potential for further integration into mesh-independent computational mechanics problems.

[Publication Link](http://dx.doi.org/10.2139/ssrn.5713427)

---

**Machine Learning Algorithms for predicting crack propagation**

A machine learning model is proposed to predict the brittle fracture of polycrystalline graphene under tensile loading. The model employs a convolutional neural network, bidirectional recurrent neural network, and fully connected layer to process the spatial and sequential features. The spatial features are grain orientations and location of grain boundaries whereas sequential features are associated with the crack growth. Molecular dynamics modeling is used to obtain the fracture process in pre-cracked polycrystalline graphene sheet subjected to tensile loading. The data from molecular dynamic simulations along with novel image-processing techniques are used to prepare the data set required to train and test the proposed model. Crack growth obtained from the machine learning model shows a close agreement with the molecular dynamic simulations. The proposed machine learning model predicts crack growth instantaneously avoiding the computational costs associated with molecular dynamics simulations.

[Publication link](https://doi.org/10.1016/j.commatsci.2021.110878)  
[GitHub link](https://github.com/MohanElapolu/poly_graph)

---

#### Relevant Publications

- Mohan S R Elapolu, Mahmoud Dinar, and Alireza Tabarraei, *FiGNNet: A Fracture-informed Graph Transformer-Attention Neural Network for Simulating Crack Propagation*, Computational Material Science (2025)
- Mohan S R Elapolu, Md Imrul Reza Shishir, and Alireza Tabarraei, *A Novel Approach for Studying Crack Propagation in Polycrystalline Graphene using Machine Learning Algorithm*, Computational Material Science (2022)
- Shishir, Md Imrul Reza, Mohan S R Elapolu, and Alireza Tabarraei, *A deep learning model for predicting mechanical properties of polycrystalline graphene*, Computational Materials Science 218 (2023)
- Kurtz, Michael A., Ruoyu Yang, Dinghe Liu, Mohan S R Elapolu, Rahul Rai, and Jeremy L. Gilbert, *Deep Neural Network Predicts Ti‐6Al‐4V Dissolution State Using Near‐Field Impedance Spectra*, Advanced Functional Materials (2023)
- Kurtz, Michael A., Ruoyu Yang, Mohan S R Elapolu, Audrey C. Wessinger, William Nelson, Kazzandra Alaniz, Rahul Rai, and Jeremy L. Gilbert, *Predicting Corrosion Damage in the Human Body Using Artificial Intelligence: In Vitro Progress and Future Applications*, Orthopedic Clinics (2023)

</div>

<div id="t2" class="tab-content" markdown="1">

#### Relevant Publications

- Mohan S R Elapolu, Alireza Tabarraei, *Mechanical and Fracture Properties of Polycrystalline Graphene with Hydrogenated Grain Boundaries*, The Journal of Physical Chemistry C (2021)
- Shishir, Md Imrul Reza, Mohan S R Elapolu, and Alireza Tabarraei, *Investigation of fracture and mechanical properties of monolayer C3N using molecular dynamic simulations*, Mechanics of Materials 160 (2021)
- Mohan S R Elapolu, Alireza Tabarraei, *Atomistic Simulation-Based Cohesive Zone Law of Hydrogenated Grain Boundaries of Graphene*, The Journal of Physical Chemistry C (2020)
- Mohan S R Elapolu, Alireza Tabarraei, *An Atomistic Study of the Stress Corrosion Cracking in Graphene*, The Journal of Physical Chemistry A (2020)
- Mohan S R Elapolu, Alireza Tabarraei, *Phononic Thermal Transport Properties of C3N nanotubes*, Nanotechnology (2019)
- Mohan S R Elapolu, Alireza Tabarraei, *Fracture mechanics of multi-layer molybdenum disulfide*, Engineering Fracture Mechanics (2019)
- Mohan S R Elapolu, Alireza Tabarraei, *Kapitza Conductance of Symmetric tilt grain boundaries of monolayer hexagonal boron nitride*, Computational Materials Science (2018)

</div>

<div id="t3" class="tab-content" markdown="1">

**Blockchain Technology for Requirement Traceability**

Requirement engineering (RE), a systematic process of eliciting, defining, analyzing, and managing requirements, is a vital phase in systems engineering. In RE, requirement traceability establishes the relationship between the artifacts and supports requirement validation, change management, and impact analysis. Establishing requirement traceability is challenging, especially in the early stages of a complex system design, as requirements constantly evolve and change. Moreover, the involvement of distributed stakeholders in system development introduces collaboration and trust issues.

This paper outlines a novel blockchain-based requirement traceability framework that includes a data acquisition template and graph-based visualization.

[Publication Link](https://doi.org/10.1016/j.is.2024.102384)  
[GitHub link](https://github.com/MohanElapolu/Blockchain-Technology-for-Requirement-Traceability-in-Systems-Engineering)

---

***Polyominoes for design***

Many computational design methods like generative models and topology optimization find optimal structures for certain requirements by iteratively trying alternatives that may include non-manifolds and without an explicit trace of feasible structures along the search. These methods focus on achieving one solution at a time. We propose a new computational framework that constructs a surrogate dataset of physically realizable designs by finding polyomino structures—neighboring squares with at least one common edge—with breadth-first search of a quadtree. We conduct Finite-Element Analysis (FEA) on each level of the tree to narrow down acceptable structures under a given load condition. Considering that all possible options for filling an n*n grid are 2n*n combinations, we use few heuristics, e.g., ignoring structures with fewer cells than the length of the bounding box, that significantly reduce the search space from trillions to thousands in our case study of an 8*8 grid. Our exhaustive yet tractable dataset of structures evaluated with FEA allows us to not only find a Pareto frontier of compliant structures but also facilitates exploring structures with different topology at the same volume fraction to adapt designs to other requirements such as support structure when additively manufactured. We demonstrate a case for bending load.

[Publication Link](https://doi.org/10.1115/DETC2025-169088)

---

#### Relevant Publications

- Mohan S R Elapolu, Rahul Rai, David J. Gorsich, Denise Rizzo, Stephen Rapp, and Matthew P. Castanier, *Blockchain technology for requirement traceability in systems engineering*, Information Systems 123 (2024)
- Mohan S R Elapolu, Mahmoud Dinar, *Design for Compositional Manufacturing in the Circular Economy*, ASME IDETC/CIE (2025)
- Mohan S R Elapolu, Mahmoud Dinar, *Creating an Exhaustive Surrogate Dataset of Polyomino Structures for Tractable Design Exploration*, ASME IDETC/CIE (2025)
- Mukunda Puvva, Mohan S R Elapolu, Mahmoud Dinar, *Adaptive Metamorphic Polyomino Structures*, ASME IDETC/CIE (2025)

</div>


</div>

<script>
function switchTab(id, btn) {
  document.querySelectorAll('.tab-content').forEach(el => el.classList.remove('active'));
  document.querySelectorAll('.tab-row button').forEach(b => b.classList.remove('active'));

  document.getElementById(id).classList.add('active');
  btn.classList.add('active');
}
</script>

</section>

<!-- PROJECTS SECTION -->
<section id="projects" markdown="1">

## Projects

**Agentic RAG Document QA Bot**
We developed a RAG based agentic model to create QA bot that acts as an interface between users and LLM (ChatGPT). This is built using LangChain and associated tool stack.  
- API calls to OpenAI models through Langchain Prompts
- Different LangChain conversation memory features
- Different LangChain Prompt Chains
- Create vector databases of document
- Built an agent to converse taking the information in document as context 

[GitHub link](https://github.com/MohanElapolu/Agentic-RAG-Document-QA-Bot.git)  

**Nanochat** 
Built the LLM from scratch and performed pretraining based on the Andrej Karpathy Nanochat project.

[GitHub link](https://github.com/MohanElapolu/nanochat.git)  

</section>

<!-- GO TO TOP BUTTON -->
<style>
  #goTopBtn {
    position: fixed;
    bottom: 30px;
    right: 30px;
    background: #0366d6;
    color: white;
    border: none;
    padding: 12px 16px;
    border-radius: 50%;
    font-size: 20px;
    cursor: pointer;
    display: none;
    box-shadow: 0px 2px 6px rgba(0,0,0,0.3);
    transition: opacity 0.3s;
  }

  #goTopBtn:hover {
    background: #024a9a;
  }
</style>

<button id="goTopBtn" onclick="scrollToTop()" title="Go to top">↑</button>

<script>
  const goTopBtn = document.getElementById("goTopBtn");

  function showGoTop() {
    goTopBtn.style.display = "block";
  }

  function hideGoTop() {
    goTopBtn.style.display = "none";
  }

  // Show button on scroll
  window.addEventListener("scroll", function () {
    if (window.scrollY > 50) {
      showGoTop();
    } else {
      hideGoTop();
    }
  });

  // Show button when navigating to an anchor (like #research)
  window.addEventListener("hashchange", function () {
    showGoTop();
  });

  // Smooth scroll to top
  function scrollToTop() {
    window.scrollTo({ top: 0, behavior: "smooth" });
  }

  // If page loads with a hash (like https://.../#research)
  if (window.location.hash) {
    showGoTop();
  }
</script>

</div>
