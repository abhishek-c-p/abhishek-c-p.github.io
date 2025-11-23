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
  - Introductory physics labs for life-science and pre-med students  
  - University physics labs for science and engineering majors  

I enjoy designing explanations, problem sets, and lab activities that connect physics ideas to real-world contexts and
students' everyday intuition.

## Example: LaTeX-rendered equations

Inline example: the kinematic equation  
$s(t) = \frac{1}{2} a t^2 + v_0 t + s_0$.

Display equation:

$$
F = m a
$$

A slightly more complex one:

$$
I = \int_{-\infty}^{\infty} e^{-x^2}\, dx = \sqrt{\pi}
$$

## Example: showing LaTeX *code* for students to copy

```latex
\begin{equation}
s(t) = \frac{1}{2} a t^2 + v_0 t + s_0
\end{equation}
```



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
