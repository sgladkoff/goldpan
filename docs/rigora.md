# Rigora: The Ultrapowerful QA Tool

**Rigora** is an ultrapowerful desktop localization QA tool.

Built on top of decades of localization engineering experience of the Logrus software developers and engineers (and recently, completely rewritten and drastically improved), **Rigora** enables you to perform the most advanced technical and linguistic checks on localized files, to fix errors interactively, and to do so in batch mode. **Rigora** can work with entire projects, as well as with singular files, making it an extremely convenient default editor for the XLIFF file format.

It is an interactive tool, and it ranks among the most powerful tools for working with software and text content.

You can visit the official website of **Rigora** here: [www.rigora.studio](http://www.rigora.studio)

## Supported File Formats

- Common bilingual file formats (XLIFF, SDLXLIFF, TMX, TTX)

- Excel workbooks

- Configurable parsing of arbitrary XML and delimited text formats

![rigor1](rigor1.png)
*Some of the file types supported by Rigora*

## Projects

**Rigora** supports two types of projects that differ from each oher drastically, including the difference with their handling of files: projects with embedded changes and projects with in-file changes (absolute and relative). Each project may support a folder structure with possibly thousands of files, if necessary.

![rigor2](rigor2.png)

A project with embedded changes does not make any changes to its files, saving all changes to the main RIGORA file. It is possible to export its document files with changes included via the Project menu.

A project with in-file changes contains only a list of file locations and settings, with all the changes going directly into its files.

**Rigora** can also be used to simply work with a single file of a supported format without creating a project, if you so choose - possibly while associating XLIFF files with Rigora in Windows.

## Checks

**Rigora** may run a large variety - more than 300 in total - of checks on the files within its projects. Among them are:

- Common checks (punctuation, tag and placeholder matching, etc.), configurable for various language pairs

- Check for invalid characters based on the target language alphabet

- Check for partially untranslated source words

- Consistency check, direct and reverse

- TM consistency checks

- Glossary Adherence Review (GAR) with stemming support, checking against external glossaries as well as in-project (using all project translations as a glossary) to verify the correct translation of all terms

- Checks for prohibited terms

An important quality of **Rigora** is that it will load all active files into the memory. Its checks are accomplished via in-memory processing, which ensures extremely fast checking, even for very large projects comprised of thousands of files.

You can add or remove checks, as well as customize their properties from the **Checks** window:

![rigor3](rigor3.png)

You can run all the checks from your check tree at once, or choose individual checks to run.

After running a check, you can export the resulting report as an XLS file.

### Glossary Adherence Review (GAR) Checks

We've written a short list of instructions for cases where you only want to run GAR checks using a particular **TMX** file on your project.

After creating your project and adding in files, you should remove all the standard settings and leave the **Checklist** empty by using the right-click menu, like so:

![rigor_gar1](rigor_gar1.png)

The **Checks** window will become empty after this. Right-click again to create your custom checklist:

![rigor_gar2](rigor_gar2.png)

Right-click the custom checklist and select the **Add Checks** option.

In the **Add Checks** window, select the **TMX File** option within the **GAR** folder and the **Glossary Type** subfolder.

![rigor_gar3](rigor_gar3.png)

In the **TMX File** window, name your new check and select the **TMX** file.

![rigor_gar4](rigor_gar4.png)

After this, you can launch the new check by right-clicking it and selecting the **Run** option. Any other check can be launched the same way.

### In-place editing

As you run your chosen set of checks, individual errors are displayed in the **Check Results** window.  

As you walk through them, they are highlighted in the files. For each error, **Rigora** will activate the file and highlight the string that contains it. When an error is fixed, it is removed from the **Checks Results** window.

![rigor4](rigor4.png)
*Rigora finds several problems with string 11067*

![rigor5](rigor5.png)
*Rigora shows untranslated text in Japanese translations*

After an error has been fixed, **Rigora** automatically re-checks the translation unit.

Not all types of checks support in-place editing (consistency and reverse consistency checks do not).

### False Positives

You can right-click an error in Check Results windows and mark it as False Positive. The error will then be removed from the list.

### Spell Checking

**Rigora** uses the Windows 10 spell checker by default:

![rigor6](rigor6.png)
*System spell checker is on by default*

To enable this, the document language must be the default system language (check Start > Settings  > Time & Language > Language).

![rigor6](rigor7.png)

You can also use Hunspell dicrionaries, which are set up separately.

### Export / Import Features

**Rigora** is very good at exporting various file formats. For example, you can export the contents of a XLIFF file as an Excel, Word or TMX file, or export unique records only to remove duplicates.

### Additional Check Results Window Functionality for GAR

As you run GAR checks in **Rigora**, you may need to copy and paste information from the glossary into one or more translation strings.

Click on a **Check Results** string containing glossary information while holding down ALT to copy it into the clipboard. Then, you'll be able to quickly paste this information wherever you want.

## Software Updates

When translating software, **Rigora** can do 100% matching updates of software strings, autotranslate ICE matches by TMX files (“software dictionary”, translated before).

## Keeping Track of the Translation Editing History at Every Stage, for Every Document Format

It is often necessary to keep track of how an editor makes changes to the document after receiving it from the translator - as well as keeping track of the document, in general, at all stages of the translation process. This is relevant for regular editors as well as MT post-editors. CAT tools often do not keep track of who exactly changes what (sometimes they do, but the process is often inconvenient).

**Rigora** solves this issue through its new function. It is used to covnert a duolingual XLIFF file into a MS Word document containting a table with two columns: source and translation. XLIFF files can be obtained easily from most CAT tools, as they enalbe the user to export a project as a set of XLIFF files at any stage of the project. So, in order to compare two versions of a document from different stages of its project, you can simply convert the XLIFF files to the DOCX format and then use the standard document-comparing function of MS Word. If you do a XLIFF export of your CAT project after the translation is done, and then another after the editing is done, you will be able to visualize everything that the editor had deemed right to fix in every document. 

![Convert a XLIFF file into a DOCX file using the File -> Export Items option with the Word Document file type](rig1.png)
*You can convert a XLIFF file into a DOCX file using the File -> Export Items option with the Word Document file type.*

![This is what a DOCX file covnerted from XLIFF looks like.](rig2.png)
*This is what a DOCX file covnerted from XLIFF looks like.*

![Use the Review -> Compare option in MS Word to compare the changes between two DOCX files belonging to different versions of a document.](rig3.png)
*Use the Review -> Compare option in MS Word to compare the changes between two DOCX files belonging to different versions of a document.*

Most CAT sytems do not offer the means of viewing versions of a document from different project stages, let alone a convenient way to view a history of changes. Making project snapshots in XLIFF format is an easy-to-use solution, available to everyone. 

The XLIFF format is especially convenient, as it enables visualizing a history of changes made to files of any format during the translation process. If you elect to use the XLIFF-to-DOCX convertion, you will be able to:

- give edited files back to your translators for future reference, with any mistakes commented on in the DOCX files by the editors

- provide your layout designers with clearly pointed out last-minute fixes for translations

- evaluate the work of your MT post-editors

- snapshot any translations out of your CAT system and provide them to your reviewers for checking in the simple DOCX format - without the trouble of arranging their access to your CAT system (or training them in its use)

## Displaying and Editing Locked Tags in SDLXLIFF Files

You can find the **Include Locked Content** and **Save Modified Locked Content** flags in the **SDLXLIFF** section of the **Project Properties** window.

![Properties](thumbnail_image001.png)

If you want to have the locked content inside SDLXLIFF files displayed and available for editing, switch these flags to **YES**.