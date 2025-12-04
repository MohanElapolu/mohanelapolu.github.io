---
layout: default
title: "Mohan Elapolu"
nav_exclude: true
---

<!-- HOME SECTION -->
<section id="home" markdown="1">
## Latest Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}

[View all posts →](/posts/)
</section>

<!-- ABOUT SECTION -->
<section id="about" markdown="1">
## About Me
I am Mohan Elapolu, a computational scientist with deep passion about understanding and predicting physical, chemical, biological, and engineered phenomena. I solve ODE/PDE-based systems using classical numerical methods and modern machine learning tools to build high- and low-fidelity simulations for complex system behavior, design optimization, and intelligent decision-making.

I construct advanced computational tools, including finite element solvers, finite-difference molecular dynamics frameworks, and physics-guided scientific machine learning models, designed to run efficiently on high-performance computing environments. I also bring deep expertise in the modern Python and AI/ML stack, including GNNs, Transformers, generative AI (LLMs, RAG, agents), and MLOps practices for scalable deployment and workflow optimization.

I specialize in pre- and post-processing large-scale computational data using Python and scientific computing libraries to extract actionable insights and support data-driven reasoning.
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

## PINNS

**FiGNNet: A Fracture-informed Graph Transformer-Attention Neural Network for Simulating Crack Propagation**

Modeling fracture in solids remains a significant challenge in computational mechanics due to the complexity of crack initiation and propagation under mixed-mode loading. In this work, we introduce a novel fracture-informed graph neural network (GNN) framework (FiGNNet) for simulating fractures in pre-cracked elastic solids. FiGNNet couples a graph transformer network (GTF) to capture long-range interactions with a graph attention network (GAT), focusing on localized behavior near crack tips. The governing equations of linear elasticity are embedded in the loss function through their weak form, ensuring physical consistency without relying on finite element analysis (FEA) solutions: displacements or stresses. The proposed approach is validated against FEA across various benchmark problems involving center and edge cracks subjected to tensile, shear, and bending loads. FiGNNet accurately predicts displacement fields, stress distributions, and crack propagation angles across all scenarios. The proposed method offers a physics-informed machine learning framework for fracture simulation, with strong potential for further integration into mesh-independent computational mechanics problems.

[Publication Link](http://dx.doi.org/10.2139/ssrn.5713427)

---

## Computer Vision

**Machine Learning Algorithms for predicting crack propagation**

A machine learning model is proposed to predict the brittle fracture of polycrystalline graphene under tensile loading. The model employs a convolutional neural network, bidirectional recurrent neural network, and fully connected layer to process the spatial and sequential features. The spatial features are grain orientations and location of grain boundaries whereas sequential features are associated with the crack growth. Molecular dynamics modeling is used to obtain the fracture process in pre-cracked polycrystalline graphene sheet subjected to tensile loading. The data from molecular dynamic simulations along with novel image-processing techniques are used to prepare the data set required to train and test the proposed model. Crack growth obtained from the machine learning model shows a close agreement with the molecular dynamic simulations. The proposed machine learning model predicts crack growth instantaneously avoiding the computational costs associated with molecular dynamics simulations.

[Publication link](https://doi.org/10.1016/j.commatsci.2021.110878)  
[GitHub link](https://github.com/MohanElapolu/poly_graph)

---

### Relevant Publications

- Mohan S R Elapolu, Mahmoud Dinar, and Alireza Tabarraei, *FiGNNet: A Fracture-informed Graph Transformer-Attention Neural Network for Simulating Crack Propagation*, Computational Material Science (2025)
- Mohan S R Elapolu, Md Imrul Reza Shishir, and Alireza Tabarraei, *A Novel Approach for Studying Crack Propagation in Polycrystalline Graphene using Machine Learning Algorithm*, Computational Material Science (2022)
- Shishir, Md Imrul Reza, Mohan S R Elapolu, and Alireza Tabarraei, *A deep learning model for predicting mechanical properties of polycrystalline graphene*, Computational Materials Science 218 (2023)
- Kurtz, Michael A., Ruoyu Yang, Dinghe Liu, Mohan S R Elapolu, Rahul Rai, and Jeremy L. Gilbert, *Deep Neural Network Predicts Ti‐6Al‐4V Dissolution State Using Near‐Field Impedance Spectra*, Advanced Functional Materials (2023)
- Kurtz, Michael A., Ruoyu Yang, Mohan S R Elapolu, Audrey C. Wessinger, William Nelson, Kazzandra Alaniz, Rahul Rai, and Jeremy L. Gilbert, *Predicting Corrosion Damage in the Human Body Using Artificial Intelligence: In Vitro Progress and Future Applications*, Orthopedic Clinics (2023)

</div>

<div id="t2" class="tab-content" markdown="1">

### Relevant Publications

- Mohan S R Elapolu, Alireza Tabarraei, *Mechanical and Fracture Properties of Polycrystalline Graphene with Hydrogenated Grain Boundaries*, The Journal of Physical Chemistry C (2021)
- Shishir, Md Imrul Reza, Mohan S R Elapolu, and Alireza Tabarraei, *Investigation of fracture and mechanical properties of monolayer C3N using molecular dynamic simulations*, Mechanics of Materials 160 (2021)
- Mohan S R Elapolu, Alireza Tabarraei, *Atomistic Simulation-Based Cohesive Zone Law of Hydrogenated Grain Boundaries of Graphene*, The Journal of Physical Chemistry C (2020)
- Mohan S R Elapolu, Alireza Tabarraei, *An Atomistic Study of the Stress Corrosion Cracking in Graphene*, The Journal of Physical Chemistry A (2020)
- Mohan S R Elapolu, Alireza Tabarraei, *Phononic Thermal Transport Properties of C3N nanotubes*, Nanotechnology (2019)
- Mohan S R Elapolu, Alireza Tabarraei, *Fracture mechanics of multi-layer molybdenum disulfide*, Engineering Fracture Mechanics (2019)
- Mohan S R Elapolu, Alireza Tabarraei, *Kapitza Conductance of Symmetric tilt grain boundaries of monolayer hexagonal boron nitride*, Computational Materials Science (2018)

</div>

<div id="t3" class="tab-content" markdown="1">

## Requirement Engineering

**Blockchain Technology for Requirement Traceability**

Requirement engineering (RE), a systematic process of eliciting, defining, analyzing, and managing requirements, is a vital phase in systems engineering. In RE, requirement traceability establishes the relationship between the artifacts and supports requirement validation, change management, and impact analysis. Establishing requirement traceability is challenging, especially in the early stages of a complex system design, as requirements constantly evolve and change. Moreover, the involvement of distributed stakeholders in system development introduces collaboration and trust issues.

This paper outlines a novel blockchain-based requirement traceability framework that includes a data acquisition template and graph-based visualization.

[Publication Link](https://doi.org/10.1016/j.is.2024.102384)  
[GitHub link](https://github.com/MohanElapolu/Blockchain-Technology-for-Requirement-Traceability-in-Systems-Engineering)

---

## Design Optimization

Many computational design methods like generative models and topology optimization find optimal structures for certain requirements by iteratively trying alternatives that may include non-manifolds and without an explicit trace of feasible structures along the search.

[Publication Link](https://doi.org/10.1115/DETC2025-169088)

---

### Relevant Publications

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
