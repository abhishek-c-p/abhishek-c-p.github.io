---
layout: page
title: Teaching
---

<!-- MathJax for LaTeX support on this page -->
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

## Teaching experience

- Graduate Teaching Assistant, Wayne State University  
  - Physics for Life Sciences 1 & 2 (Introductory course for non-majors)
  - University Physics for Scientists and Engineers 1 & 2 (Introductory course for majors)
- Lab instructor
  - Physics for Life Sciences 1 lab (Experiments dealing with directed and random motion at the microscopic level)
  - Descriptive astronomy (Learning about planetary motion and the night sky using available data)




<style>
  .testimonial-marquee {
    position: relative;
    overflow: hidden;
    width: 100%;
    padding: 1rem 0;
    margin-top: 0.5rem;

    /* soft fade at edges */
    mask-image: linear-gradient(to right, transparent, black 8%, black 92%, transparent);
    -webkit-mask-image: linear-gradient(to right, transparent, black 8%, black 92%, transparent);
  }

  .testimonial-track {
    display: flex;
    gap: 1.5rem;
    width: max-content;
    animation: testimonial-scroll 140s linear infinite;
    align-items: center;
  }

  .testimonial-track img {
    height: 260px;
    width: auto;
    border-radius: 14px;
    box-shadow: 0 8px 24px rgba(0,0,0,0.45);
    transition: transform 0.2s ease;
  }

  .testimonial-track img:hover {
    transform: translateY(-4px) scale(1.02);
  }

  @keyframes testimonial-scroll {
    from { transform: translateX(0); }
    to   { transform: translateX(-50%); }
  }

  @media (prefers-reduced-motion: reduce) {
    .testimonial-track { animation: none; }
  }

  @media (max-width: 768px) {
    .testimonial-track img { height: 200px; }
  }
</style>

<div class="testimonial-marquee" aria-label="Student teaching evaluations carousel">
  <div class="testimonial-track">
    {% for i in (1..20) %}
      {% if i < 10 %}
        {% assign num = "0" | append: i %}
      {% else %}
        {% assign num = i %}
      {% endif %}
      <img src="/assets/img/testimonials/quote_dark_wsu_{{ num }}.jpg"
           alt="Student teaching evaluation {{ i }}">
    {% endfor %}

</div>


## Teaching Philosophy 


The purpose of education is not simply to memorize facts, but to shape how students think. In physics especially, learning should rewire the brain toward critical reasoning, curiosity, and problem-solving. My goal as an educator is to help students engage with the physical world, build logical thinking habits, and leave the classroom more confident in their ability to make sense of complex ideas.

#### Building critical thinking through connections

To cultivate scientific reasoning, I focus on helping students see connections across topics and develop a “big-picture” view of physics. Traditional learning can feel like isolated islands of knowledge, so I consistently show how ideas relate and build into a coherent framework.

One practice I use in every class is spending the first 5–10 minutes revisiting a challenging problem from the previous lecture or homework. We break it into smaller steps, discuss how to choose the right concepts and equations, and reflect on common pitfalls. This routine strengthens understanding while steadily building student confidence.

#### Engagement through collaboration and support

Student engagement is central to my teaching. I incorporate group activities and peer learning because students often grasp ideas faster when they explain them to each other. At the same time, I provide individual support through personalized feedback and regular office hours. Balancing collaborative learning with one-on-one guidance ensures every student has multiple ways to succeed.

#### Adapting to diverse learners

Over the past four years, teaching has been one of the most rewarding parts of my graduate life. I’ve worked with both majors and non-majors, and these experiences have taught me how to adapt my approach to different needs.

In **Physics for Life Sciences I & II**, many students come from biology or medical backgrounds with limited math preparation. I introduce concepts in a math-light way at first, then gradually bring in the necessary tools—like vectors—so they can confidently handle forces and Newton’s laws.

In **University Physics for Scientists and Engineers I & II**, the focus shifts toward a deeper theoretical foundation. Rather than jumping straight into formulas, I guide students through the physical reasoning that leads to the mathematics, helping them appreciate why the equations look the way they do.

In laboratory courses, I emphasize hands-on learning and real-time data analysis so students can connect abstract ideas to measurable experience. Tools such as interactive simulations (e.g., PhET) further help students with different levels of familiarity engage meaningfully with the material.

#### Creating an inclusive, compassionate classroom

An inclusive and supportive classroom environment is essential to learning. I strive to develop equitable practices that resonate with students from diverse backgrounds and ensure that all students feel seen, valued, and capable. My graduate coursework in college-level teaching has strengthened my ability to design learning spaces that welcome different perspectives and learning styles.

I also believe effective teaching must be grounded in compassion and patience. Learning is a journey, and students grow best when they feel safe to struggle, ask questions, and improve at their own pace. I aim to meet students where they are, encourage them through challenges, and give them the grace to learn without fear.

#### Continual growth and motivation

I am committed to improving as an educator by staying informed about pedagogical innovations and thoughtfully integrating them into my teaching. What motivates me most is seeing the moment when a student finally “gets it”—whether it’s understanding why the sky is blue or realizing how Newton’s laws shape everyday life.

Those moments remind me why I teach. With the right guidance, every student can grow into a curious, logical thinker prepared to engage the world with rigor and wonder. My commitment is to help students grow not only academically, but also as confident, critical individuals ready to explore the universe through physics.



<style>
  .testimonial-marquee {
    position: relative;
    overflow: hidden;
    width: 100%;
    padding: 1rem 0;
    margin-top: 0.5rem;

    /* soft fade at edges */
    mask-image: linear-gradient(to right, transparent, black 8%, black 92%, transparent);
    -webkit-mask-image: linear-gradient(to right, transparent, black 8%, black 92%, transparent);
  }

  .testimonial-track {
    display: flex;
    gap: 1.5rem;
    width: max-content;
    animation: testimonial-scroll 140s linear infinite;
    align-items: center;
  }

  .testimonial-track img {
    height: 260px;
    width: auto;
    border-radius: 14px;
    box-shadow: 0 8px 24px rgba(0,0,0,0.45);
    transition: transform 0.2s ease;
  }

  .testimonial-track img:hover {
    transform: translateY(-4px) scale(1.02);
  }

  @keyframes testimonial-scroll {
    from { transform: translateX(0); }
    to   { transform: translateX(-50%); }
  }

  @media (prefers-reduced-motion: reduce) {
    .testimonial-track { animation: none; }
  }

  @media (max-width: 768px) {
    .testimonial-track img { height: 200px; }
  }
</style>

<div class="testimonial-marquee" aria-label="Student teaching evaluations carousel">
  <div class="testimonial-track">
    {% for i in (1..20) %}
      {% if i < 10 %}
        {% assign num = "0" | append: i %}
      {% else %}
        {% assign num = i %}
      {% endif %}
      <img src="/assets/img/testimonials/quote_dark_wsu_{{ num }}.jpg"
           alt="Student teaching evaluation {{ i }}">
    {% endfor %}

    <!-- Duplicate for seamless loop -->
    {% for i in (1..20) %}
      {% if i < 10 %}
        {% assign num = "0" | append: i %}
      {% else %}
        {% assign num = i %}
      {% endif %}
      <img src="/assets/img/testimonials/quote_dark_wsu_{{ num }}.jpg" alt="">
    {% endfor %}
  </div>
</div>
