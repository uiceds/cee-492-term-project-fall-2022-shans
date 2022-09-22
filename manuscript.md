---
title: Rail Track Change Detection Based On Components' Health Conditions
keywords:
- markdown
- publishing
- manubot
lang: en-US
date-meta: '2022-09-22'
author-meta:
- Arthur Bilheri
- negin Shafie
- Shirin Qiam
- Sadaf Shafie
header-includes: |-
  <!--
  Manubot generated metadata rendered from header-includes-template.html.
  Suggest improvements at https://github.com/manubot/manubot/blob/main/manubot/process/header-includes-template.html
  -->
  <meta name="dc.format" content="text/html" />
  <meta name="dc.title" content="Rail Track Change Detection Based On Components&#39; Health Conditions" />
  <meta name="citation_title" content="Rail Track Change Detection Based On Components&#39; Health Conditions" />
  <meta property="og:title" content="Rail Track Change Detection Based On Components&#39; Health Conditions" />
  <meta property="twitter:title" content="Rail Track Change Detection Based On Components&#39; Health Conditions" />
  <meta name="dc.date" content="2022-09-22" />
  <meta name="citation_publication_date" content="2022-09-22" />
  <meta name="dc.language" content="en-US" />
  <meta name="citation_language" content="en-US" />
  <meta name="dc.relation.ispartof" content="Manubot" />
  <meta name="dc.publisher" content="Manubot" />
  <meta name="citation_journal_title" content="Manubot" />
  <meta name="citation_technical_report_institution" content="Manubot" />
  <meta name="citation_author" content="Arthur Bilheri" />
  <meta name="citation_author_institution" content="Hogwarts school of witchcraft" />
  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />
  <meta name="twitter:creator" content="@I dont like birds" />
  <meta name="citation_author" content="negin Shafie" />
  <meta name="citation_author_institution" content="Department of Civil and Environmental Engineering, University of Illinois at Urbana-Champaign" />
  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />
  <meta name="twitter:creator" content="@NA" />
  <meta name="citation_author" content="Shirin Qiam" />
  <meta name="citation_author_institution" content="Department of Civil and Environmental Engineering, University of Illinois at Urbana-Champaign" />
  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />
  <meta name="twitter:creator" content="@NA" />
  <meta name="citation_author" content="Sadaf Shafie" />
  <meta name="citation_author_institution" content="Department of Civil and Environmental Engineering, University of Illinois at Urbana-Champaign" />
  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />
  <meta name="twitter:creator" content="@NA" />
  <link rel="canonical" href="https://uiceds.github.io/cee-492-term-project-fall-2022-shans/" />
  <meta property="og:url" content="https://uiceds.github.io/cee-492-term-project-fall-2022-shans/" />
  <meta property="twitter:url" content="https://uiceds.github.io/cee-492-term-project-fall-2022-shans/" />
  <meta name="citation_fulltext_html_url" content="https://uiceds.github.io/cee-492-term-project-fall-2022-shans/" />
  <meta name="citation_pdf_url" content="https://uiceds.github.io/cee-492-term-project-fall-2022-shans/manuscript.pdf" />
  <link rel="alternate" type="application/pdf" href="https://uiceds.github.io/cee-492-term-project-fall-2022-shans/manuscript.pdf" />
  <link rel="alternate" type="text/html" href="https://uiceds.github.io/cee-492-term-project-fall-2022-shans/v/4f7d9c34e881b6313647e681634aeda2746821ee/" />
  <meta name="manubot_html_url_versioned" content="https://uiceds.github.io/cee-492-term-project-fall-2022-shans/v/4f7d9c34e881b6313647e681634aeda2746821ee/" />
  <meta name="manubot_pdf_url_versioned" content="https://uiceds.github.io/cee-492-term-project-fall-2022-shans/v/4f7d9c34e881b6313647e681634aeda2746821ee/manuscript.pdf" />
  <meta property="og:type" content="article" />
  <meta property="twitter:card" content="summary_large_image" />
  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />
  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />
  <meta name="theme-color" content="#ad1457" />
  <!-- end Manubot generated metadata -->
bibliography:
- content/manual-references.json
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
manubot-clear-requests-cache: false
...






<small><em>
This manuscript
([permalink](https://uiceds.github.io/cee-492-term-project-fall-2022-shans/v/4f7d9c34e881b6313647e681634aeda2746821ee/))
was automatically generated
from [uiceds/cee-492-term-project-fall-2022-shans@4f7d9c3](https://github.com/uiceds/cee-492-term-project-fall-2022-shans/tree/4f7d9c34e881b6313647e681634aeda2746821ee)
on September 22, 2022.
</em></small>

## Authors



+ **Arthur Bilheri**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [artbil94](https://github.com/artbil94)
    · ![Twitter icon](images/twitter.svg){.inline_icon}
    [I dont like birds](https://twitter.com/I dont like birds)<br>
  <small>
     Hogwarts school of witchcraft
  </small>

+ **negin Shafie**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [negins2](https://github.com/negins2)
    · ![Twitter icon](images/twitter.svg){.inline_icon}
    [NA](https://twitter.com/NA)<br>
  <small>
     Department of Civil and Environmental Engineering, University of Illinois at Urbana-Champaign
     · Funded by none
  </small>

+ **Shirin Qiam**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [Shirin-qiam](https://github.com/Shirin-qiam)
    · ![Twitter icon](images/twitter.svg){.inline_icon}
    [NA](https://twitter.com/NA)<br>
  <small>
     Department of Civil and Environmental Engineering, University of Illinois at Urbana-Champaign
     · Funded by none
  </small>

+ **Sadaf Shafie**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [sadafs2](https://github.com/sadafs2)
    · ![Twitter icon](images/twitter.svg){.inline_icon}
    [NA](https://twitter.com/NA)<br>
  <small>
     Department of Civil and Environmental Engineering, University of Illinois at Urbana-Champaign
     · Funded by none
  </small>



## Abstract {.page_break_before}




## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
