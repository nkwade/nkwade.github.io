---
title: "GEDCOM2Wiki"
date: 2025-01-10T20:28:35-04:00
draft: false
---

`gedcom2wiki` converts GEDCOM files into a set of HTML pages representing a Wikipedia-style family tree. It generates an index page, pages for each family, pages for each individual, and a data validation report. The goal is to make it easy to share and explore family trees without relying on online genealogy services which often have bad viewing UI anyways. <!--more--> As of Jan. 10th 2025 over 100 people have viewed my code, 20 have cloned it, and 5 have starred my repo. It has been great seeing people make use of a passion project of mine. My geneology is something I have poured countless hours into and combining it with my programming abilities has been a great exercise. 

[Github Repo](https://github.com/nkwade/gedcom2wiki)

[Example Output Of The Royal Family](https://wade.dev/static/royaltreewiki/index.html)

## Quick Stats
- Initial Public Release: January 2025
- Primary Use: Family Tree Browsing & Data Validation
- Lines of Python Code: ~1500
- Optimized to parse trees in under 1 second and generated a Wiki in seconds


## Tech Stack
- Python  
- HTML Templating for Wiki pages  
- Command line interface with argparse  
- Pickle for caching
- MyPy for static typing
- Black for auto-formatting
- Github for source control and presenting to the public

## How It Works
1. **GEDCOM Parsing:** The script reads and parses the GEDCOM file to build `Fact` objects. It then organizes those facts into a `FamilyTree` data structure.  
2. **Family Tree Parsing** Once a `FamilyTree` has a list of facts, they are split into list of facts for every person and family which then parse themselves into a usable object. 
2. **Optional Caching:** You can store or retrieve the parsed tree from a cache file to speed up subsequent runs.  
3. **Wiki Generation:** Using the `FamilyTree` object the program creates HTML pages for each person, family, and source, plus an index and optional validation page. It writes these files to the specified output folder.  
4. **Viewing the Result:** Open the generated `index.html` (found in your output folder) in a browser to explore the Wiki-style pages.  

