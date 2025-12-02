---
layout: default
title: "Mohan Elapolu"
nav_exclude: true
---

<style>
  body {
    scroll-behavior: smooth;
  }
  section {
    padding: 40px 0;
    border-bottom: 1px solid #ddd;
  }
  h2 {
    margin-top: 40px;
  }
</style>

<nav class="site-nav" style="margin-bottom: 40px;">
  <a href="#home">Home</a> |
  <a href="#about">About</a> |
  <a href="#research">Research</a> |
  <a href="#projects">Projects</a>
</nav>

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
Hi, I'm **Mohan**.

- AI / ML  
- Research  
- Writing

I enjoy learning, building, and publishing my thoughts online.
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
    <button class="active" onclick="switchTab('t1', this)">Topic 1</button>
    <button onclick="switchTab('t2', this)">Topic 2</button>
    <button onclick="switchTab('t3', this)">Topic 3</button>
  </div>

  <!-- TAB CONTENT SECTIONS -->
  <div id="t1" class="tab-content active" markdown="1">
### Topic 1  
Your content for topic 1…
  </div>

  <div id="t2" class="tab-content" markdown="1">
### Topic 2  
Your content for topic 2…
  </div>

  <div id="t3" class="tab-content" markdown="1">
### Topic 3  
Your content for topic 3…
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

**Machine Learning Algorithms for predicting crack propagation**
A machine learning model is proposed to predict the brittle fracture of polycrystalline graphene under tensile loading. The model employs a convolutional neural network, bidirectional recurrent neural network, and fully connected layer to process the spatial and sequential features. The spatial features are grain orientations and location of grain boundaries whereas sequential features are associated with the crack growth. Molecular dynamics modeling is used to obtain the fracture process in pre-cracked polycrystalline graphene sheet subjected to tensile loading. The data from molecular dynamic simulations along with novel image-processing techniques are used to prepare the data set required to train and test the proposed model. Crack growth obtained from the machine learning model shows a close agreement with the molecular dynamic simulations. The proposed machine learning model predicts crack growth instantaneously avoiding the computational costs associated with molecular dynamics simulations.
[GitHub link](https://github.com/MohanElapolu/poly_graph)

**Blockchain Technology for Requirement Traceability** 
Requirement engineering (RE), a systematic process of eliciting, defining, analyzing, and managing requirements, is a vital phase in systems engineering. In RE, requirement traceability establishes the relationship between the artifacts and supports requirement validation, change management, and impact analysis. Establishing requirement traceability is challenging, especially in the early stages of a complex system design, as requirements constantly evolve and change. Moreover, the involvement of distributed stakeholders in system development introduces collaboration and trust issues. This paper outlines a novel blockchain-based requirement traceability framework that includes a data acquisition template and graph-based visualization. The template enables dual-level traceability (artifact and object) in the RE processes. The traceability information acquired through the templates is stored in the blockchain, where traces are embedded in blocks’ metadata and data. Furthermore, the blockchain is represented as a Neo4J property graph where traces can be retrieved using Cypher queries, thus enabling a mechanism to query and examine the history of requirements. The framework’s efficacy is showcased by documenting the RE process of an autonomous automotive system. Our results indicated that the framework can record the history of artifacts with constantly changing requirements and can yield secure decentralized ledgers of requirement artifacts. The proposed distributed traceability framework has shown promise to enhance stakeholder collaboration and trust. However, additional user studies should be conducted to bolster our results.
[GitHub link](https://github.com/MohanElapolu/Blockchain-Technology-for-Requirement-Traceability-in-Systems-Engineering)  


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