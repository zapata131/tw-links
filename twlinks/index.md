---
layout: default
---

# 🔗 [Technical Writing links](/)

A simple page with useful resources for technical writers in the software
industry.

[Learn more about the project](/about.html).

<nav class="section-nav" aria-label="Sections">
  <ul>
    <li><a href="#guides">Guides</a></li>
    <li><a href="#tools">Tools</a></li>
    <li><a href="#courses">Courses</a></li>
    <li><a href="#books">Books</a></li>
    <li><a href="#blogs">Blogs</a></li>
    <li><a href="#podcasts">Podcasts</a></li>
    <li><a href="#videos">Videos</a></li>
    <li><a href="#communities">Communities</a></li>
  </ul>
</nav>

---

## {% include icon.html name="guides" %} Guides & Case Studies {#guides}

- [Docs as Code (Write the Docs Guide)](https://www.writethedocs.org/guide/docs-as-code/):
  A practical primer on treating documentation with the same tools and workflows
  as source code—Markdown, Git, code reviews, and CI/CD.
- [Diátaxis](https://diataxis.fr/): A systematic framework by Daniele Procida
  that divides documentation into four types: tutorials, how-to guides,
  reference, and explanation. It's a useful mental model for thinking about
  docs, though I have my reservations about how strictly it's sometimes applied
  in practice.
- [GitHub Docs (Open Source Repo)](https://github.com/github/docs): The actual
  repository behind GitHub's documentation. A great real-world reference if you
  want to see how a large team structures content, style rules, and docs-as-code
  workflows at scale.
- [Writing for Web Accessibility (W3C)](https://www.w3.org/WAI/tips/writing/): A
  short, actionable checklist from the W3C covering headings, link text, alt
  text, and clear instructions. Easy to apply right away.
- [Growth.Design Case Studies](https://growth.design/case-studies): While
  focused on UX, these "comic book" style case studies are incredible for
  learning how to write concise, persuasive interface copy.
- [Ask me about API docs](https://askmeaboutapis.com/): A unique page written by
  Clarence William Cromwell that has a set of guides and essays, for both
  developers and technical writers, about writing API documentation.
- [OpenAPI Learning Portal](https://learn.openapis.org/): The official guide
  from the OpenAPI Initiative. A clear, structured reference for understanding
  and writing OpenAPI specifications.

## {% include icon.html name="tools" %} Tools & Reference {#tools}

- [Google developer documentation style guide](https://developers.google.com/style/):
  A complete style guide for technical writers. Highly suggested if you are a
  solo writer or starting a technical writing team. (Don't reinvent the wheel.)
- [The Good Docs Project](https://www.thegooddocsproject.dev/): Provides
  best-practice templates and checklists for various types of technical
  documentation (READMEs, API refs, etc.).
- [Merriam-Webster.com](https://merriam-webster.com): For all your spelling needs.
- [Markdown Guide](https://www.markdownguide.org/): A clean, no-nonsense cheat
  sheet and reference for Markdown syntax. Useful to keep bookmarked (or to
  share with engineers contributing to your docs).
- [The Art of Command Line](https://github.com/jlevy/the-art-of-command-line):
  Useful if you need to be fluent in using the command line in *NIX systems.
- [Excalidraw](https://excalidraw.com/): A free, open-source virtual whiteboard
  with a hand-drawn look. Great for putting together quick architecture diagrams
  and flows without fighting heavy diagramming tools.
- [Mermaid](https://mermaid.js.org/): Diagrams as code. It lets you write
  flowcharts, sequence diagrams, and architecture graphs right inside your
  Markdown files so they stay version-controlled with the rest of your docs.
- [Vale](https://vale.sh/): An open-source "linter for prose." It allows you to
  enforce your style guide (like Google or Microsoft) automatically within your
  code editor.
- [Doc Detective](https://docs.doc-detective.com/): An open-source testing framework
  for documentation. Lets you automatically verify that your UI steps, CLI
  commands, and API calls still match how the product actually behaves.
- [llms.txt](https://llmstxt.org/): A lightweight Markdown convention for making
  your documentation easy for LLMs and AI coding agents to read. Worth keeping
  on your radar as more developers consume docs through AI tools.

## {% include icon.html name="courses" %} Courses {#courses}

- [Google's Technical writing courses](https://developers.google.com/tech-writing/overview):
  Four courses about the basics of technical writing, including writing for
  accessibility and writing error messages.
- [Learn Git Branching](https://learngitbranching.js.org/): An interactive,
  visual sandbox for learning Git. Very useful if you are getting started with
  docs-as-code and want to feel comfortable with branches, rebasing, and merges.
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/):
  A course by Tom Johnson, the author of the I'd Rather be Writing blog. A
  complete guide to learn everything you need to know about REST APIs,
  documenting endpoints, using the OpenAPI spec, and more.

## {% include icon.html name="books" %} Books {#books}

### Technical writing

- [Modern Technical Writing: An Introduction to Software Documentation](https://www.amazon.com/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS/):
  By Andrew Etter. A short, practical introduction to lightweight software
  documentation principles and workflows.
- [Docs for Developers](https://www.amazon.com/Docs-Developers-Engineers-Technical-Writing-ebook/dp/B09HLZGWKT/):
  By Jared Bhatti, Jen Lambourne, David Nunez, et al. An engineer-friendly field
  guide covering the full documentation lifecycle, from planning and drafting to
  publishing and maintenance.
- [Docs Like Code](https://www.docslikecode.com/book/): By Anne Gentle. A
  hands-on guide to applying software development tools and workflows—like Git,
  code reviews, and automated builds—to documentation.
- [Every Page is Page One](https://xmlpress.net/publications/eppo/): By Mark
  Baker. The book behind the topic-based writing approach for web documentation.
- [Docs as Tests](https://www.docsastests.com/): By Manny Silva. Introduces a
  strategy for treating documentation like software tests so your examples and
  guides don't quietly go stale.
- [The Product is Docs](https://www.amazon.com/Product-Docs-technical-documentation-development-ebook/dp/B085KHTV95/):
  By Christopher Gales and the Splunk Documentation Team. Practical lessons on
  building, scaling, and running a documentation team alongside product
  development.
- [Documentation at Scale](https://www.amazon.com/dp/B0HGPRKYMN): By Andrew
  Etter. A follow-up to *Modern Technical Writing* focused on building and
  scaling documentation strategies in the AI era.

> *Note: To learn more about some of these books, you can read the
> [Three books to boost your technical writing career](https://bufferbuffer.com/three-books-to-boost-your-technical-writing-career/)
> post.*

### APIs and UX writing

- [Web API Design Crafting Interfaces that Developers Love](https://www.academia.edu/11335664/Web_API_Design_Crafting_Interfaces_that_Developers_Love):
  By Brian Mulloy. This book with a Creative Commons license is a good read if
  you want to get involved in helping design and document REST APIs.
- [Strategic Writing for UX](https://www.amazon.com/Strategic-Writing-Engagement-Conversion-Retention/dp/1492049395/):
  By Torrey Podmajersky. A solid foundation if you are involved with UX writing
  or want to learn more about the subject.
- [Microcopy: The Complete Guide](https://www.microcopybook.com/): By Kinneret
  Yifrah. A great companion to *Strategic Writing for UX* packed with real-world
  examples of buttons, empty states, onboarding, and error messages.

## {% include icon.html name="blogs" %} Blogs {#blogs}

- [I'd Rather be Writing](https://idratherbewriting.com/): Written by Tom
  Johnson, a technical writer working at Google. He has interesting post series
  about different topics related to technical writing.
- [Passo Uno](https://passo.uno/): Written by Fabrizio Ferri Benedetti, a
  technical and UX writer working at Elastic. His posts vary from editorial
  pieces to in-depth discussions about the current state of technical writing.
- [This is important](https://thisisimportant.net/): Written by Sarah Moir, a
  technical writer at Sigma. Her unique vision of combining data analysis and
  technical writing, plus the way she guides you through her thinking process,
  make this blog an interesting read.
- [Docs Like Code blog](https://www.docslikecode.com/): Anne Gentle's site and
  blog on docs-as-code practices, developer portals, and modern documentation
  workflows.
- [Every Page is Page One blog](https://everypageispageone.com/): Mark Baker's
  blog challenging traditional linear documentation and teaching how to write
  for the way users actually search on the web.

## {% include icon.html name="podcasts" %} Podcasts {#podcasts}

- [The Not-Boring Tech Writer](https://thenotboringtechwriter.com/): A
  down-to-earth podcast about the real day-to-day of technical writing—tools,
  career paths, imposter syndrome, and working with engineers.
- [Write the Docs Podcast](https://podcast.writethedocs.org/): Panel-style
  conversations with practitioners talking about documentation culture, tools,
  and lessons learned.
- [The Cherryleaf Podcast](https://www.cherryleaf.com/podcast/): Hosted by Ellis
  Pratt, featuring interviews and discussions about technical communication,
  managing doc teams, and how AI is changing the field.

## {% include icon.html name="videos" %} Videos {#videos}

- [What nobody tells you about documentation](https://www.youtube.com/watch?v=p0PPtdRHG6M):
  By Daniele Procida for Write the Docs Prague 2017. The talk that introduced
  the Diátaxis framework—a must-watch for anyone thinking about how to structure
  docs.
- [How to write the perfect error message](https://www.youtube.com/watch?v=hzCfl8CGJuw):
  By James Scott for Write the Docs Prague. Good for every writer.
- [Treating Documentation like Code: a Practical Account](https://www.youtube.com/watch?v=Mzu-c-FoOdw):
  By Jodie Putrino for Write the Docs Portland 2017. A practical look at
  adopting developer workflows for documentation.
- [Minimum Viable Documentation for RESTful APIs](https://www.youtube.com/watch?v=E3YesNMUx1o):
  By Mike Jang for API the Docs 2020. Covers the essentials every REST API needs
  to get developers up and running.
- [Beyond spell checking - what else can we check automatically?](https://www.youtube.com/watch?v=8NukYx5ggCM):
  By Tony Ibbs. An interesting talk about automation with a DocOps approach to
  technical writing.
- [Write inclusive, people-first language about AI](https://www.youtube.com/watch?v=wH3H8ko43gM):
  By Alexandra Klepper for Write the Docs. A talk on how to describe AI features
  clearly and inclusively, without the hype. (Alexandra is my coworker, and she
  is really nice.)
- [Proving and improving the value of your docs](https://www.youtube.com/watch?v=4PuZV1j5M0E):
  By Tal Gluck for Write the Docs. A practical talk on choosing documentation
  metrics that actually matter to leadership and help improve doc quality.
- [Write the Docs YouTube Channel](https://www.youtube.com/@writethedocs):
  Hundreds of talks from Write the Docs conferences around the world, covering
  everything from Docs-as-Code to AI and content strategy.

## {% include icon.html name="communities" %} Communities & Conferences {#communities}

- [Write the Docs](https://www.writethedocs.org/): "A global community of people
  who care about documentation." They organize annual conferences in Portland,
  Berlin, Kenya, and Australia, and meetups across the globe. The page has some
  interesting resources and a wholesome Slack community.
- [API the Docs](https://apithedocs.org/): An online conference focusing
  exclusively on API documentation.
- [tcworld conference](https://tcworldconference.tekom.de/): The largest annual
  conference for technical communication, held every fall in Stuttgart, Germany.
  It leans a bit more traditional than Write the Docs, but it has solid tracks
  on structured content, compliance, and AI in tech comm.
