# [**Introduction link**](https://zhenggao.io/blog/2019/12/10/Jekyll-%E6%90%AD%E5%BB%BA%E4%B8%AA%E4%BA%BA%E7%BD%91%E7%AB%99/ "blog"): 👈

# TODO:

```markdown
<!-- in _includes/footer/custom.html -->

<!-- in _pages/sitemap.md -->

# Finish it!!!!!!!!!!!!

<!-- in _pages/publication.md -->


<!-- in _pages/cv.md -->
<!-- 想要网页版不要下载版，就注释掉cv.html，把cv.md上的注释取消 -->

---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

## EDUCATION

**Huazhong University of Science and Technology**, Hubei, China

**⋄**  **B.S. in Computer Science**, expected July 2024 2020 - Present

**⋄**  **Cumulative GPA:** 3.85 / 4.00

## EXPERIENCE

**Intern Student**,  Jun 2022 - Present

Distributed Systems Team, Key Laboratory of Service Computing and Systems Ministry of Education & Amp, Huazhong Uni. of Science & Tech., *Wuhan, Hubei, China*

- Co-led the research of extending the sandwich arbitrage strategy to a "Lasagne" strategy.
- Carried out several experiments to achieve substantial optimization of arbitrage speed and accuracy.
- Developed an arbitrage system for the "Lasagne" strategy using Node.js, TypeScript, Go, and solidity.
- Led a "XETH" project: An open-source platform for Ethereum data intelligence analysis and management.

**Intern Student**,  Jan 2022 - Feb 2022 & Jul 2022 - Present

PDSL team, Wuhan photoelectric national research center parallel data storage laboratory, *Wuhan, Hubei, China*

- Participated in the Talent Plan of PingCAP company and completed the tinykv project.
- Joined the DPU-KV group to do some research on offloading distributed applications to the DPU.

**Intern Student**,  Oct 2020 - Nov 2021

Key Laboratory of Digital Manufacturing Equipment and Technology, *Wuhan, Hubei, China*

- Optimized the Apriltag vision algorithm using C++.
- Developed a desktop application tracking and displaying the robot's position in real time using Qt, C++, and CSS.
- Prepared for the 17th "Challenge Cup" National Competition.

## AWARDS & SCHOLARSHIPS

**⋄  First Prize**: 17th "Challenge Cup" National College Student Curricular Academic Science & Technology Works Competition, *Apr 2022*

**⋄  Grand Prize**: 13th Hubei Province "Challenge Cup" College Student Curricular Academic Science & Technology Works Competition, *May 2021*

**⋄  Grand Prize**: 8th "Qiushi Cup" College Student Academic Science & Technology Works Competition, *Apr 2021*

**⋄  First Prize**: 17th "Mindray Cup" College Student Robot Competition, *Apr 2021*

**⋄**  School Merit Student Scholarship, *Oct 2021*

**⋄**  School Innovation Scholarship, *Oct 2022*

**⋄**  National Hisense Scholarship, *May 2022*

**⋄**  National Huawei's "Smart Base" Scholarship, *May 2022*

**⋄**  School Freshman Excellence Scholarship, *Apr 2021*

**⋄**  School Freshman Self-improvement Scholarship, *Apr 2021*

## PUBLICATIONS

**Lasagne: Exploring More Profitable Opportunities in Blockchain** *(Revised)*

## SOCIETY MEMBERSHIPS

**Team Dian**, Hubei, China

- Leader of Web Group, *Sep 2021 - Present*
- Led a "kidpose" project, built team wiki and the official website.

**Team FOCUS**, Hubei, China

- Leader, *Oct 2020 - Present*
- Daily organization and management of the team.
- Led projects about amphibious robots and the web.
- Led the Preparation for the 17th "Challenge Cup" National Competition.

**Team STAR**, Hubei, China

- Member, *Sep 2021 - Present*
- Research on databases and distributed key-value storage.

**Organization Department of the School Youth Committee**, Hubei, China

- Assistant of the Comprehensive Management Office, *Oct 2020 - Oct 2021*
- Organized large-scale conferences and cultural and sports activities.
- Coordinated the work of departments of the committee.
- Volunteer activities including Campus Health Maintenance and Hometown cleaning.
- Social practice activities including high-school presentations and the "Three Rural Areas" Social Practice.
- Gained the prize of **School Excellent Practice Individual** in July 2021.
#PUBLICATIONS

<ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

# Skills

* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3

# Publications

  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

# Talks

  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>

# Teaching

  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

# Service and leadership

* Currently signed in to 43 different slack teams

```

A Github Pages template for academic websites. This was forked (then detached) by [Stuart Geiger](https://github.com/staeiou) from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the MIT License. See LICENSE.md.

I think I've got things running smoothly and fixed some major bugs, but feel free to file issues or make pull requests if you want to improve the generic template / theme.

### Note: if you are using this repo and now get a notification about a security vulnerability, delete the Gemfile.lock file.

# Instructions

1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
2. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right.
3. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
4. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
5. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.
6. Check status by going to the repository settings, in the "GitHub pages" section
7. (Optional) Use the Jupyter notebooks or python scripts in the `markdown_generator` folder to generate markdown files for publications and talks from a TSV file.

See more info at https://academicpages.github.io/

## To run locally (not on GitHub Pages, to serve on your own computer)

1. Clone the repository and made updates as detailed above
2. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
3. Run `bundle clean` to clean up the directory (no need to run `--force`)
4. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
5. Run `bundle exec jekyll liveserve` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.

# Changelog -- bugfixes and enhancements

There is one logistical issue with a ready-to-fork template theme like academic pages that makes it a little tricky to get bug fixes and updates to the core theme. If you fork this repository, customize it, then pull again, you'll probably get merge conflicts. If you want to save your various .yml configuration files and markdown files, you can delete the repository and fork it again. Or you can manually patch.

To support this, all changes to the underlying code appear as a closed issue with the tag 'code change' -- get the list [here](https://github.com/academicpages/academicpages.github.io/issues?q=is%3Aclosed%20is%3Aissue%20label%3A%22code%20change%22%20). Each issue thread includes a comment linking to the single commit or a diff across multiple commits, so those with forked repositories can easily identify what they need to patch.
