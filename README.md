# Using the Master Bibtek File
The master bibtek file that can be added to all new edpr latex projects to keep a single, curated, source for citing well!

 - Create a new overleaf project for your paper. Use a blank template and upload the style files, or overleaf's inbuilt templates, for the conference/journal to which you wish to submit. The repository must be called **YEAR_LASTNAME_VENUE**
 - In the new repository click _New File_ ➡️ _ _From External URL_ . The URL is **XX** and the name should be **edpr-bib.bib**
 - Use the edpr_bib.bib along with \usepackage{biblatex} for citing work. The citation format is **author_year_{letter}**. FYI the letter is added when multiple author/year combinations occur.
 - Add new references to the imported edpr-bib.bib directly in your overleaf project
 - When the project is submitted, got to **githuburl**, edit the master edpr-bib.bib file and add any missing references you added to your overleaf project so they are available for you and others in the next publication!
