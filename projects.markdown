---
layout: page
title: Projects
permalink: /projects/
---

<html>
              <script id="MathJax-script" async
                src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
        </script>
        <h2>Menu</h2>
        <p>
        <ul>
          <li><a href="#onehealth">Air Quality and One Health AI Prediction</a></li>
          <li><a href="#ljp">Post-Hoc Interpretability for Legal Judicial Prediction Models</a></li>
          <li><a href="#cmi">MIT PRIMES CrowdMath Internship</a></li>
          <li><a href="#mlviol">Violence Surveillance Detection with Ensemble Learning</a></li>
          <li><a href="mechinterp">Mechanistic Interpretability</a></li>
          <li><a href="#problemtrainer">Problems Trainer</a></li>
          <li><a href="#som">Self-Organizing Map Applications</a></li>
          <li><a href="#flf">Fractional Linear Functions</a></li>
          <li><a href="#writingspeaking">Writing and Speaking</a></li>
        <div id = "onehealth">
        <h2>Air Quality and One Health AI Prediction</h2>
        <p>Mentored by <a href="https://zihengsun.github.io/">Dr. Ziheng Sun</a>, I'm working on a project that hopes to find the best AI model that can predict the risk score for one region to certain diseases (lung cancer, other air quality related cancers) using remote sensing. We have cleaned data for AQI's of different counties, HPAI outbreaks in birds, radon information, and lung cancer data. Our next step is to improve our models and run interpretability tests. Here is the <a href="https://github.com/earth-artificial-intelligence/one_health_assip_2025">GitHub Repo</a>.</p>
        </div>
        <div id = "ljp">
        <h2>Post-Hoc Interpretability for Legal Judicial Prediction Models</h2>
        <p>Mentored by <a href="https://uk.linkedin.com/in/michael-maslowski-16546a255">Michael Maslowski</a>, I'm working on a project that hopes to increase transparency of AI judicial prediction models. Currently three are not that many AI applications to the legal system put into practical use because AI currently functions largely like a black box. Hence, we hope to apply post-hoc interpretability techniques like SHAP (SHapley Additive exPlanations) address this by providing insight into how different features in the data affect the predictions. SHAP in particular is a powerful and popular technique as it provides global interpretability across the data-set, as well as local interpretability for a particular decision.</p>

        <p>However SHAP’s main vulnerability is adversarial perturbation, which is when an agent manipulates input features, makes minor adjustments or introduces random noise to change feature importance or SHAP values significantly. Thus, SHAP should be robust, that is the feature importance or SHAP values should remain the same even after minor perturbations and introduction of random noise. SHAP has been found to be robust in precision medicine, especially for simpler models. However, there is a gap in evaluating SHAP in the judicial sector and more complex models.</p>

        <p>In this project we aim to evaluate the robustness of SHAP in more complex models in the judicial sector, using publicly available judicial models. We compare the SHAP Values of a control set of normal inputs against the SHAP Values of a set of perturbed inputs (simulating gradient based adversarial attacks with FGSM) or inputs with added noise.</p>
        <p>Here is the <a href="https://github.com/annadeng8/ljp-interp">GitHub Repo</a>.</p>
        </div>
        <div id="cmi">
        <h2>MIT PRIMES CrowdMath Internship</h2>
        <p>Our project focuses on exploring the <a href="https://artofproblemsolving.com/polymath/mitprimes2025">CrowdMath 2025</a> open problems while leveraging AI tools such as Large Language Models and interactive theorem provers. We are working towards providing the first taxonomy of classes of commutative rings/semirings based on the statement of Goldbach’s conjecture using AI+math workflows with reusable AI enhancement techniques. Our mentors for this project are <a href="https://math.mit.edu/~fgotti/">Dr. Felix Gotti (MIT)</a>, <a href="https://www.marlygotti.com/">Dr. Marly Gotti (Arcus Biosciences)</a>, and <a href="https://joseph.vulakh.us/">Joseph Vulakh (MIT)</a>.</p>
        <p>In the reading period of the project, my team and I worked on developing abstract algebra and AI tools. We have been enhancing our understanding of both the additive and multiplicative structures in semidomains, dealing with notions like atomicity, Furstenberg-ness, and MCD/GCD. We have specifically focused on the cyclic "natural" semidomain \(\mathbb{N}_0[\alpha]\) for \(\alpha\in \mathbb{Q}\) and in general algebraic \(\alpha\). We also have been working on open problems regarding the lesser-known multiplicative monoid of \(\mathbb{N}_0[\alpha]^*\). In the AI component, we have worked on fine-tuning and prompt-engineering GPT models to create AI assistants that can aid with looking up concepts, checking understandings, and coming up with proofs for our project. We have also worked on some basic Lean usage through the <a href="https://adam.math.hhu.de/#/g/leanprover-community/nng4">Natural Numbers Game</a>. </p>
        <p>In a semidomain, an atom is an irreducible element. We say an atom is strong if any integer multiple (\(c\) times an atom) of the atom is likewise irreducible (i.e. it cannot be written as a sum of other atoms besides the \(c\) copies of the atom). </p>
        <p>In the active research period of the project, we investigated realizable pairs of \( |(\mathcal{S}(\mathbb{N}_0[\alpha])|, |\mathcal{A}(\mathbb{N}_0[\alpha]))| \), and our main result was in finding the \(\alpha\) that realized pairs of the form \( (4k+c, 5k+c)\) for all \((k,c) \in \\mathbb{N} \times \mathbb{N}_0\). We also developed algorithms to compute the unique canonical sum decomposition of an element in \(\mathbb{N}_0[\alpha]\), the number of strong atoms and atoms of \(\mathbb{N}_0[\alpha]\), and so on.</p>
        <p>We also looked into the multiplicative structure of \(\mathbb{N}_0[q]\) for rational \(q\). In particular, we classified when \(\mathbb{N}_0[q]\) has the properties of unique factorization, bounded factorization, and finite factorization. </p>
        <p>We will be presenting our findings at the <a href="https://intrepid-math.com/">Summer Workshop for Intrepid Mathematicians</a> (SWIM) 2025. </p>
        <p>Here is the <a href="https://github.com/marlycormar/cmi-2025">GitHub repo</a>.</p>
        </div>
        <div id="mlviol">
        <h2>Violence Surveillance Detection with Ensemble Learning</h2>
        <p>This project dives into developing a model for detecting violent actions from video clips taken from surveillance cameras. We seek to balance both model accuracy and model efficiency to ensure violence on camera both correctly and quickly creates alerts to those who can help, like law enforcement or other people located in other parts of the building. One such model is a three-stage deep learning-based end-to-end framework with a lightweight convolutional neural network for identifying individuals in frame and a 3D-CNN model that extracts the spatiotemporal features of these sequences, which are finally passed into a classifier. The model is trained on <a href="https://github.com/annadeng8/violence-detection-datasets">a variety of datasets</a>, including the Hockey-Fight Dataset and RWF-2000 dataset, and cross-data experiments will be performed.</p>
        </div>
        <div id="mechinterp">
        <h2>Mechanistic Interpretability</h2>
        <p>As an individual project, I've been exploring more about the field of mechanistic interpretability and AI safety in general. For the Non-Trivial Research Foundations program, I drafted a proposal for a research project involving applying fractal analysis to mechanistic anomaly detection. This <a href="https://github.com/annadeng8/anom-detect-fractal">GitHub Repo</a> contains my work on it so far! As part of the Algoverse AI research program, I am working on a project involving applying semantic entropy probes to improve judge models, inspired by <a href="https://arxiv.org/abs/2406.15927">this paper</a>.</p>
        <p>Now a bit about mech interp in general—read this paper <a href="https://distill.pub/2020/circuits/zoom-in/">Zoom In</a> to get started. There are three speculative claims about neural networks: 1. features, directions in the activation space representing properties of the input, are the fundamental unit of analysis. 2. features are connected into circuits via network weights, and these circuits often have meaning. 3. features and circuits are universal across models, i.e. the universality hypothesis. There is also the concept of superposition, which says that a model can represent more features than there are dimensions in its hidden space, thus "cramming" multiple features into a single neuron, which can lead to polysemantic neurons that can be hard to interpret. </p>
        </div>
        <div id="problemtrainer">
        <h2><a href="https://www.problemstrainer.app/about">Problems Trainer</a></h2>
            <p>personalized competition math trainer developed in collaboration with Yourui Shao and Helen Peng using Python web frameworks, HTML/CSS, SQL, NLP</p>
            <ul><li>Source past AMC problems adaptively to improve practicing efficiency, evaluating users’ strengths and weaknesses with problem types and categories and subsequently recommend such problems.</li>
              <li>Use of machine learning to categorize problems gathered via webscraping.</li></ul>
            <h3><a class="fa fa-star"></a> What makes this trainer different <a class="fa fa-star"></a></h3>
              <video muted width="500" height="140" autoplay="autoplay"> <source src="https://www.problemstrainer.app/static/media/answering_problem.mp4" type="video/mp4" />Entering an answer</video>
              <video muted width="300" height="150" autoplay="autoplay"> <source src="https://www.problemstrainer.app/static/media/category_selection.mp4" type="video/mp4" />Selecting categories to practice exclusively</video>
            <p><li>Recommendations – we recommend problems at your difficulty level based on your scores (though the metrics for calculating difficulty could be improved).</li>
              <li>Profiles – feel rusty and want to restart your progress? No need to create a new account!</li>
              <li>Quantitative performance – we keep track of your progression in accuracy with handy score calculations.</li>
              <li>Faster categorization – We train natural language processing models to categorize problems, which allow easy classification of problems from other contests so we can begin to incorporate them.</li>
            </p>
            </div>
        <div id="som">
        <h2>Self-Organizing Maps</h2>
        <p>A <a href="https://en.wikipedia.org/wiki/Self-organizing_map">self-organizing map (SOM)</a> is an unsupervised machine learning technique used to produce a low-dimensional (typically two-dimensional) representation of a higher-dimensional data set while preserving the topological structure of the data.</p>
        An SOM is trained using competitive learning. Upon being fed a training example, the SOM finds the neuron that is closest to the input (best matching unit or BMU). Then the weights of the BMU and the neighboring neurons are updated to become more similar to the input. 
        <p>The update formula is as follows:
        \(W_v(s+1)=W_v(s)+\theta(u,v,s)\cdot\alpha(s)\cdot(D(t)-W_v(s))\)
        where \(\theta\) is the neighborhood function, \(\alpha\) is the learning rate parameter, and \(D(t)-W_v(s)\) is the distance between the target input and the current weight.
        The neighborhood function allows the areas closest to the BMU to be updated more than the those farther away. The learning rate slowly decreases so the map updates more in the beginning rather than at the end.
        </p>
        <p>As part of the Laurienzo research group, I investigated applications of self-organizing maps in many areas, including building efficient rail networks, displaying knots, and image classification.</p>
        <h3>Knots</h3>
        <p>Classifying knots has been researched extensively. In the mathematical field of knot theory, <a href="https://en.wikipedia.org/wiki/Knot_invariant">knot invariants</a> such as <a href="https://en.wikipedia.org/wiki/Knot_polynomial">knot polynomials</a> 
        have been found to distinguish knots, but these methods may be computationally challenging.</p>
        <p>We generated SOMs of various knots. This can be used for knot identification as seen in the promising heatmaps, a topic that has applications in computational biology and DNA.</p>
        <p>Here is a figure 8 knot with the nodes of the SOM. The rightmost image shows four angles of the heatmap of nodes. Comparisons of this heatmap can show distinctions between the knot types.</p>
        <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Blue_Figure-Eight_Knot.png"  width="300" height="300" >
        <img src="/images/8knot.png" width="310" height="305">
        <img src="/images/8knotheatmaps.png" width="310" height="305">
        <p>Here is a pretzel knot.</p>
        <img src="https://math201s09.wikidot.com/local--files/dewey-knot/goodknot.bmp" width="300" height="300">
        <img src="/images/pretzel.png" width="310" height="305">
        <img src="/images/pretzelheatmaps.png" width="310" height="305">
        <h3>Rail Networks</h3>
        <p>In this project, our motivation was to output a rail system that minimized the average time needed to travel between any two points in the network based on a dataset of the areas' population. This is especially useful for planning transportation networks in developing countries.
          Below is the process of generating an SOM on the U.S. population. We start with our population dataset and a grid of 5x5 nodes (our SOM size). Then we used the SOM algorithm to adjust the nodes to match those of the dataset. Finally we connected the edges (railways!).
        </p>
        <img src="/images/usapopdata.png" width="230" height="230">
        <img src="/images/usadatasetinitialnodes.png" width="230" height="230">
        <img src="/images/usadatasetnodes.png" width="230" height="230">
        <img src="/images/usanodeswithedges.png" width="230" height="230">
        <p>Next, we went through a pruning process on the edges to minimize a cost function. At each step we would remove an \(n\)th edge, then add it back, and out of all possible \(n\)th edge removals, we would finally remove the edge that gave the least cost. Below is a cost vs. edges removed graph.</p>
        <img src="/images/usaoptimizedstat.png" width="420" height="260">
        <p>Some other experiments with our designed algorithms included testing a hexagonal SOM vs. square initialization. There were not many noticeable differences, though the hexagonal SOM had more edges and therefore took more time. The below images show pruning on the first and last iterations of the hexagonal grid.</p>
        <img src="/images/usabeginningedges.png" width="337" height="313">
        <img src="/images/usaedgesremoved.png" width="337" height="313">
        <p>We also added considerations for altitude in our cost calculations based on the USA's geographic elevation dataset, as traveling uphill or drilling a tunnel takes significantly more resources. Similar experiments were conducted on other country datasets, including those of developing countries. See the slides <a href="assets/somrailslides.pdf">linked here</a> for more experiments done.</p>
      </div>
        <div id="flf">
        <h2>Fractional Linear Functions</h2>
        <a href="/Fractional_Linear_Functions.pdf">Download Paper</a>
        <p>Fractional linear functions are functions \(f\) of the form \(\frac{ax+b}{cx+d}\). 
          They have many important applications, including their usefulness as transformations, constructing the hyperbolic plane, and even in Andrew Wile's proof of Fermat's Last Theorem. 
          At PROMYS this summer, I teamed up with other math enthusiasts in investigating the properties of fractional linear functions without any outside sources, hence the name "exploration lab." 
          Here are some interesting results we proved in the above paper:
        <ul><li>If \(f\) has order \(n\) then the possible cycle lengths of elements in \(\mathbb{P}_p\) are divisors of \(n\).</li>
          <li>Every fractional linear function on \(\mathbb{P}_p\) has a cycle length which divides \(p^2-1\) or is exactly \(p\). (using matrix diagonalization and splitting fields)</li>
        <li>There are \((p-1)^2(p+1)(p)\) fractional linear functions without simplification. (using the orbit-stabilizer theorem)</li>
      <li>... and many more!</li></ul></p>
      <p>On one of the final days of the program, my group gave a presentation! Here are the <a href="/Fractional_Linear_Functions_slides.pdf">slides</a> to our presentation.</p>
        <img src="/images/promysflfgroup.jpg" width="403" height="302" alt="flfgroup">
        </div>
        <div id = "writingspeaking">
          <h2>Writing and Speaking</h2>
          <ul>
            <li><a href="https://monotonicallyincreasing.substack.com/">my Substack titled "monotonically increasing"!</a></li>
            <li><a href="https://docs.google.com/document/d/1n5SVqRir0UUVJlrhlvEdeDY7O-P-QDG2w9mNPa-8Dlk/edit?usp=sharing">Why Worry about Women in STEM?</a> - a piece of writing I submitted to the Scholastic Awards in the Personal Essay category that won a regional Honorable Mention.</li>
            <li><a href="https://docs.google.com/document/d/1s6F3JxUsh7-y5vW0tYk4lEVLQKezd_hYe7GCYQbxAO8/edit?tab=t.0">a TED Talk about my TED Talk</a></li>
            <li><a href="https://www.canva.com/design/DAGUDu5QWvU/ZogfmfpAo613fmtiMHs0TA/view?utm_content=DAGUDu5QWvU">A.I.M. for Education - proposed artificial intelligence framework in schools</a></li>
            <li><a href="https://docs.google.com/document/d/1SvLWCOyNso-uoijYUL1kx_VNICNSiolSJY_r8D9YOJE/edit?usp=sharing">TED Talk Script 2024</a>: delivered on May 3, 2024 <a href="https://www.youtube.com/watch?v=_UgkzdZAeXk">here</a></li>
            <li><a href="https://docs.google.com/document/d/1oYixuAlnvhpxMgNN7f-zFXhzsagvzuSCCF5y1r1yg_E/edit?usp=sharing">TED Talk Script 2025</a>: delivered on March 21, 2025</li>
            </ul>
            <br>
        </div>
