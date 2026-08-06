---
title: "About"
layout: gridlay
sitemap: false
permalink: /about/
---

## About

<div class="section-card">
<div class="pi-card">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ site.photo }}" class="pi-photo" alt="{{ site.name }}" loading="lazy">
<div>
<h3 class="pi-name">{{ site.name }}</h3>
<p style="font-style: italic; color: var(--text-secondary);">{{ site.title }}, {{ site.institution }}</p>
<div class="pi-links">
{% if site.email %}<a href="mailto:{{ site.email }}" class="icon-link" title="Email"><i class="fa-solid fa-envelope"></i></a>{% endif %}
{% if site.links.cv and site.links.cv != "" %}<a href="{{ site.url }}{{ site.baseurl }}/{{ site.links.cv }}" class="icon-link" title="CV"><i class="ai ai-cv"></i></a>{% endif %}
{% if site.links.google_scholar and site.links.google_scholar != "" %}<a href="{{ site.links.google_scholar }}" class="icon-link" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>{% endif %}
{% if site.links.github and site.links.github != "" %}<a href="{{ site.links.github }}" class="icon-link" title="GitHub"><i class="fa-brands fa-github"></i></a>{% endif %}
{% if site.links.researchgate and site.links.researchgate != "" %}<a href="{{ site.links.researchgate }}" class="icon-link" title="ResearchGate"><i class="ai ai-researchgate"></i></a>{% endif %}
</div>
{% if site.data.pi[0].education %}
<ul style="margin-top: var(--space-4);">
{% for education in site.data.pi[0].education %}
<li>{{ education | replace: "-","&#8211;" }}</li>
{% endfor %}
</ul>
{% endif %}
</div>
</div>
</div>

<div class="section-card">

<h3>Research Appointments</h3>

**Graduate researcher, Stanford University** (2023–present)

- Adviser: [Alison Marsden](https://profiles.stanford.edu/alison-marsden), Co-adviser: [Gianluca Iaccarino](https://profiles.stanford.edu/gianluca-iaccarino)
- Developing multi-fidelity parameter estimation methods for interventional planning of peripheral pulmonary artery stenosis (PPAS).

**Undergraduate researcher (senior thesis), California Institute of Technology** (2022-23)

- Adviser: [Tim Colonius](https://www.eas.caltech.edu/people/colonius)
- Developed a two-dimensional data-driven reduced-order model of burst-wave lithotripsy to determine optimal frequencies to break kidney stones
- Thesis: Towards a Reduced-Order Model of Burst-Wave Lithotripsy

**Undergraduate summer research fellow, Massachusetts Institute of Technology** (Summer 2022)
- Adviser: [Themis Sapsis](https://meche.mit.edu/people/faculty/sapsis@MIT.EDU)
- Combined Bayesian optimization, extreme acquisition functions, and an ensemble of deep neural operators to predict rogue waves in high dimensions and jet acoustic bursts. ([Abstract](https://sfp.caltech.edu/documents/22774/Compiled_Abstract_Book_22_ioVhgnc.pdf))

**Undergraduate summer research fellow, California Institute of Technology** (Summer 2021)
- Adviser: [Tim Colonius](https://www.eas.caltech.edu/people/colonius)
- Analyzed optimized eddy-viscosity models for coherent structures in the first and second azimuthal modes of turbulent jets and examined the physical significance of the approach to mechanisms present in the jet. ([Abstract](https://sfp.caltech.edu/documents/19869/Compiled_Summer_Abstracts.pdf))

**Undergraduate summer research fellow, California Institute of Technology** (Summer 2020)
- Adviser: [Julia Greer](https://www.eas.caltech.edu/people/jrgreer)
- Investigated the fibrous properties of the A. aurita jellyfish mesoglea to characterize the viscoelastic response under flat punch indentation and to model radial symmetrization. ([Abstract](https://sfp.caltech.edu/documents/17703/Final_Abstract_Book_for_Posting_937lr6m.pdf))

**High school intern, Massachusetts Institute of Technology** (Summer 2018)
- Adviser: [Kerri Cahoy](https://aeroastro.mit.edu/people/kerri-cahoy/)
- Modified a receiver assembly for MIT's Portable Telescope for Lasercom (PorTeL) to improve tracking performance. Successful IR camera photo of the International Space Station was presented by a graduate student at the 2018 SmallSat Conference.
- Note: As of 2022, my modified version of the receiver assembly is still working and set up in MIT Wallace Astrophysical Observatory

</div>

{% if site.data.awards %}
<div class="section-card">
<h3>Awards</h3>
<ul>
{% for award in site.data.awards %}
<li>{{ award.name | replace: "-","&#8211;" }}</li>
{% endfor %}
</ul>
</div>
{% endif %}

<div class="section-card">
<h3>Professional Memberships</h3>
- American Heart Association (AHA) (2025-)
- Stanford Cardiovascular Institute (CVI) (2025-)
- Society for Industrial and Applied Mathematics (SIAM) (2024-)
- American Physical Society (APS) (2021-)

</div>

{% if site.data.grants %}
<div class="section-card">
<h3>Grants</h3>
<ul>
{% for grant in site.data.grants %}
<li>{{ grant.name }}</li>
{% endfor %}
</ul>
</div>
{% endif %}

{% if site.data.people %}
<div class="section-card">
<h3>Students and Mentoring</h3>
<ul>
{% for student in site.data.people %}
<li>{{ student.name }}, {{ student.location }} ({{ student.degree }}, {{ student.year }})</li>
{% endfor %}
</ul>
</div>
{% endif %}

{% if site.data.funders %}
<div class="section-card">
<h4>Sponsors</h4>
<div class="sponsor-logos" style="display: flex; flex-wrap: wrap; align-items: center; justify-content: center; gap: var(--space-6);">
{% for funder in site.data.funders %}
<a href="{{ funder.url }}" target="_blank"><img src="{{ site.url }}{{ site.baseurl }}/images/{{ funder.image }}" alt="Funder logo" style="max-height: 80px; max-width: 200px; border-radius: 0;" loading="lazy"></a>
{% endfor %}
</div>
</div>
{% endif %}
