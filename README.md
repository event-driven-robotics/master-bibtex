# 📚 Using the Master BibTeX File

The master BibTeX file can be added to all new EDPR LaTeX projects to keep a single, curated source for well-formatted citations.

---

* **🛠️ Create your LaTeX project:** Use a blank template and upload the style files, or Overleaf's inbuilt templates, for the conference/journal to which you wish to submit. The repository must be called **YEAR_LASTNAME_VENUE**

* **🌐 Add the master bibliography file:** In the new repository click `New File ➡️ From External URL`. The URL is
  ```
  https://raw.githubusercontent.com/event-driven-robotics/master-bibtex/refs/heads/main/test.bib
  ```
   and the name should be `edpr-bib.bib`

* **🧠 Using BibTeX:** If you are unfamiliar with BibTeX, consider [a quick tutorial](https://www.overleaf.com/learn/latex/Bibliography_management_with_bibtex). The citation format is **author_year_{letter}** i.e. `\cite{bartolozzi_2026f}` and Overleaf should give autocomplete for paper titles, so we hope it is simple to find the correct paper to cite. 💡 The letter is added when multiple author/year combinations occur. The bibliography is added to the paper using:
  ```latex
  \bibliographystyle{plain}
  \bibliography{edpr-bib}
  ```
  💡 Replace the *plain* style with the style in your conference/journal style files.

* **🔄 Update the BibTeX file:** New citations that are not yet in the `.bib` file can be added directly to the [github .bib file](https://github.com/event-driven-robotics/master-bibtex/blob/main/test.bib). Edit the file directly in the github online interface, and make a commit directly to main branch. After you add your new reference, in your Overleaf click 🖱️ `edpr-bib.bib ➡️ Refresh`.

* **🛠️ Rules for generating labels for bibliography entries:
  1. for multiple authorsin year 20XX: FirstAuthor_etalXX 
  2. for two authors: FirstAuthor_SecondAuthorXX
  3. for single author: AuthorXX
  4. add venue acronym if there are multiple papers in the same year (e.g. tnnls, icra, tcas, natcomm, etc.)

* Notes: if the paper has capitalized acronyms use $$; make sure to add \ if there are special characters; make sure to always include the paper DOI.
