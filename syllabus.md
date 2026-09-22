---
layout: default
title: "Syllabus"
---

<nav class="card toc" aria-label="On this page" markdown="1">
**On this page:** [Description](#description) · [Learning outcomes](#outcomes) · [Course components](#components) · [Grading](#grading) · [Late policy](#late-policy) · [AI tools](#ai-tools) · [Academic integrity](#integrity) · [Communication](#communication) · [Materials](#materials) · [Accommodations](#accommodations) · [Student resources](#resources)
</nav>

<section class="card" markdown="1">
## Course Description {#description}

This course is a project-based introduction to computer vision: how machines acquire, process, and interpret visual information from images and video. We begin with image formation, filtering, and local features, then build to the deep learning methods behind modern vision systems, including convolutional networks, vision transformers, and vision-language models. The course pairs conceptual understanding with hands-on experiments, so you learn not only how these methods work, but why they work and when they fail.

Every assignment asks for evidence, not only an implementation: you will run experiments, read the resulting curves, test methods on data you collect yourself, and defend your choices. The final project applies the same habits to a question of your own choosing.

**Prerequisites** (minimum grade of C in each course unless noted):

* I&C SCI 6D
* MATH 3A *or* I&C SCI 6N
* MATH 2B *or* AP Calculus BC (minimum score of 4)
* I&C SCI 46
* One of COMPSCI 112, COMPSCI 116, COMPSCI 171, or COMPSCI 178

In practice you'll rely most on linear algebra, probability, and programming in Python.
</section>

<section class="card" markdown="1">
## Student Learning Outcomes {#outcomes}

Upon successful completion of the course, students should be able to:

1. Explain the core concepts of computer vision, from image formation, filtering, and feature extraction to modern deep learning representations, and analyze how visual information is encoded and processed.
2. Implement, train, and evaluate computer vision models using modern frameworks such as PyTorch, and interpret their performance using appropriate metrics and diagnostics.
3. Critically assess the strengths, limitations, and failure modes of computer vision methods, and justify design choices in written and oral communication.
4. Apply computer vision techniques to a new problem by framing a measurable question, choosing a suitable model, data, and baseline, and answering the question with honest evaluation.
</section>

<section class="card" markdown="1">
## Course Components {#components}

**Lectures** meet in person, {{ site.lecture_days }} {{ site.lecture_time }} in {{ site.lecture_location }}. Two lectures (Image Formation and Intro to Learning) are delivered as recorded videos, and those two class meetings (Oct 7 and Oct 12) are TA-led project labs. Slides and readings are posted on Canvas.

**Problem sets.** Three problem sets, each released at the lecture that unlocks it:

* P1: Images, filtering, and color
* P2: Local features and matching
* P3: CNN recognition

Each has three graded parts, weighted the same way every time:

| Part | Weight | Graded by |
|---|---|---|
| Code correctness | 45% | Hidden autograder tests |
| Experiment results | 30% | Automatic checks on the `results.json` your notebook writes |
| Report | 25% | A short list of yes/no rubric items, printed in the report template |

Reports use patterns you will see in every problem set: results on data you collect yourself, a written prediction before you run an experiment, a parameter sweep instead of a single number, and a hunt for inputs that break the method. Photos you collect are graded on being present, never on quality or on the accuracy you achieve. If a prediction turns out to be wrong, saying so earns full credit.

**Midterm.** In class on Wed, Nov 4, on paper. It covers material through Nov 2.

**Final project.** A team project that asks and answers an empirical question using open-source vision models. It runs from the Oct 7 lab to a video due Mon, Dec 7, the course's final-week activity under UCI Senate Regulation A465. See the [Project page]({{ '/project/' | relative_url }}).

**Participation.** Short required items, each available from the start of the quarter: the project seed (due Oct 11), the syllabus survey (due Oct 16), and the team roster (due Oct 16). Engagement in class, in the project labs, and on Ed Discussion also counts.
</section>

<section class="card" markdown="1">
## Grading {#grading}

| Component | Weight |
|---|---|
| Participation | 5% |
| Problem Set 1 | 10% |
| Problem Set 2 | 15% |
| Problem Set 3 | 15% |
| Midterm Exam | 20% |
| Final Project | 35% |
| **Total** | **100%** |
{: .grade-table}

Within the final project: proposal 15%, check-in 20%, presentation 20%, and video + code 45%. The project seed and team roster count toward participation. Due dates are on the [Assignments page]({{ '/assignments/' | relative_url }}).

**Grade cutoffs** (final percentage, minimum for each grade):

| Letter | Plus (e.g. A+) | Letter (e.g. A) | Minus (e.g. A−) |
|---|---|---|---|
| A | 97 | 93 | 90 |
| B | 87 | 83 | 80 |
| C | 77 | 73 | 70 |
| D | 67 | 63 | 60 |
| F | n/a | below 60 | n/a |
{: .cutoff-table}
</section>

<section class="card" markdown="1">
## Late Policy {#late-policy}

Every assignment has a **{{ site.grace_days }}-day grace period** after its deadline, unless the assignment says otherwise. Work submitted during the grace period is accepted without penalty, and you don't need to ask. **Nothing is graded after the grace period ends.**

The last accepted day for every assignment is listed on the [Assignments page]({{ '/assignments/' | relative_url }}). Exceptions are stated there too. For example, Problem Set 1 is accepted through Thu, Oct 16, for students who add the course late. Participation items and in-class presentations have no grace period.

The grace period is meant to cover the ordinary surprises of a quarter: illness, travel, interviews, clustered deadlines, computer problems. If a serious illness or emergency lasts beyond it, contact the instructor as soon as you can.
</section>

<section class="card" markdown="1">
## Use of AI Tools {#ai-tools}

Using AI coding assistants (for example ChatGPT or Claude) is **permitted and expected** in this course. It is part of how this work is done now.

Every problem set report ends with a required **AI-use disclosure**:

* which tools you used,
* roughly what you asked them, and
* **at least one specific thing the tool got wrong or misled you about, and how you caught it.**

The disclosure is not surveillance, and it carries no penalty. It is graded on specificity, because noticing where a confident tool is wrong is the actual professional skill.

What you submit must still reflect your own understanding. Your predictions, analyses, and conclusions must be your own. Presenting AI-generated work as your own thinking, or using AI tools without disclosing them, is academic dishonesty.
</section>

<section class="card" markdown="1">
## Academic Integrity {#integrity}

You are expected to pursue your studies with honesty and integrity, and to follow the [UCI Academic Integrity Policy](https://aisc.uci.edu/). Plagiarism is presenting the ideas, words, or work of another as your own without proper acknowledgment. It includes, but is not limited to:

* submitting work, in part or in whole, that was completed by another person;
* failing to cite sources for ideas, facts, code, or conclusions taken from others;
* closely paraphrasing or substantially reproducing someone else's work;
* submitting work purchased or obtained from outside sources or services.

Problem set code and reports are **individual work**. You may discuss ideas with classmates, but do not share code or post solution code on Ed Discussion. The final project builds on open-source code by design. You must separate your team's contribution from what the original repository already did (see the [Project page]({{ '/project/' | relative_url }})).

Suspected academic dishonesty is handled under UCI policy. Penalties range from a zero on the assignment to failing the course, and cases may be reported to the [Office of Academic Integrity & Student Conduct](https://aisc.uci.edu/).
</section>

<section class="card" markdown="1">
## Communication {#communication}

**Ed Discussion** is the main channel for course questions: concepts, assignments, and logistics. Posting there lets the whole course staff and your classmates answer faster, and everyone benefits from the answer. The course staff aim to respond within 24 hours on weekdays.

**Email** is for private matters, such as grading concerns or personal circumstances. Email from your UCI address, and expect a reply within 24–48 hours on business days.

**In class**, ask questions at any time. Arrive on time, use laptops and phones only for course activities, and keep discussion respectful. Disruptive or dismissive behavior will be addressed under UCI policy.
</section>

<section class="card" markdown="1">
## Materials and Technology {#materials}

**Readings** (both free online):

* *Computer Vision: Algorithms and Applications*, 2nd ed., Richard Szeliski (2022). The primary text.
* *Foundations of Computer Vision*, Antonio Torralba, Phillip Isola, and William T. Freeman (2024). Supplementary.

Links are on the [Resources page]({{ '/resources/' | relative_url }}).

**Technology:**

* A laptop that can run Python 3.11. Problem sets 1 and 2 run on the CPU of any laptop.
* Problem set 3 and most final projects need a GPU. The free tier of Google Colab is enough, and every assignment is sized to run there. Department cluster access is arranged only for final projects that need more.
* A reliable internet connection.
</section>

<section class="card" markdown="1">
## Accommodations {#accommodations}

Students who need accommodations should register with the [UCI Disability Services Center](https://dsc.uci.edu/). Share your accommodation letter with the instructor as early in the quarter as possible, and at least a week before the midterm.
</section>

<section class="card" markdown="1">
## Student Resources {#resources}

**Campus resources**

* [UCI Libraries](https://www.lib.uci.edu/)
* [Center for Excellence in Writing and Communication](https://www.writingcenter.uci.edu/)
* [Learning & Academic Resource Center (LARC)](https://www.larc.uci.edu/)
* [UCI Disability Services Center](https://dsc.uci.edu/)
* [Office of Information Technology (OIT)](https://www.oit.uci.edu/)
* [UCI Counseling Center](https://counseling.uci.edu/resources/resources-for-students/)
* [Student Affairs: Wellness, Health, and Counseling](https://studentaffairs.uci.edu/services-for-students/)
* [Office of Academic Integrity & Student Conduct](https://aisc.uci.edu/)

**Basic needs**

If you have trouble securing enough food or housing, and you believe this may affect your performance in the course, please contact the [Dean of Students](https://www.dos.uci.edu/) (949-824-5181) for support. You can also get help from:

* [Student Outreach and Retention Center (SOAR)](https://soar.uci.edu/)
* [UCI Basic Needs Center](https://basicneeds.uci.edu/), at the FRESH Basic Needs Hub, 4079 Mesa Rd

**Sexual violence and sexual harassment**

Title IX prohibits gender discrimination, including sexual harassment, domestic and dating violence, sexual assault, and stalking. If you have experienced sexual harassment or sexual violence, you can get confidential support and advocacy from the [Campus Advocacy Resources & Education (CARE) office](https://care.uci.edu/), by phone at (949) 824-7273 or by email at [care@uci.edu](mailto:care@uci.edu).

You can report incidents through the [Office of Equal Opportunity and Diversity](https://www.oeod.uci.edu/harassment_guide/index.php). OEOD also lists [sexual violence resources](https://www.oeod.uci.edu/sho/resources-sexual-violence.php) that are available even when campus is closed.

Under the [UC Policy on Sexual Violence and Sexual Harassment](https://policy.ucop.edu/doc/4000385/SVSH), faculty and TAs must notify the Title IX Office if they learn that a student has experienced sexual violence or sexual harassment.
</section>

<section class="card" markdown="1">
## Acknowledgements

The problem sets descend from Georgia Tech CS 4476/6476 and, before that, Brown CS 143 by James Hays, with contributions from Samarth Brahmbhatt, John Lambert, Judy Hoffman, Viraj Prabhu, Mitch Donley, and Vijay Upadhya. Lecture materials draw on slides by Devi Parikh, Frank Dellaert, Kristen Grauman, David Fouhey, James Hays, Derek Hoiem, and Svetlana Lazebnik. Each slide set and assignment carries its own acknowledgements. You may reuse these materials for academic or research purposes, but please keep all acknowledgements.
</section>
