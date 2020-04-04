# The primary operations available to Goldpan users.

## Creating, opening and editing multilingual translation memory (TMX) files with up to nine parallel language pairs

## Creating, opening and editing terminology (TBX) files

## Importing translation resources from the SDLTM, SDLXLIFF, XLIFF, TMX and TBX file formats:

To import translation resources from a file, open the Import/Export tab and press the Import File button. In the dialog window, select a file format from the drop-down menu, then find and select the file. This operation can only import resources from a single file per use. If necessary, employ the operation multiple times to import resources from several files.

## Exporting selected resources into TMX, XLIFF, TBX or XLSX files:

Goldpan will only export the segments present in its memory, which is populated by means of the Move to Memory and Copy to Memory buttons on the Import/Export tab. The Move to Memory operation removes any highlighted segments from the editor, but the Copy to Memory operation leaves the segments in the editor. Segments can be highlighted through commonly used operations including clicking while holding down SHIFT or CTRL, or clicking-and-dragging. Only entire segments will be moved or copied. If a segment is visible as being partially highlighted, the entire segment will still be moved or copied. An export operation can be started with the Export button, which is located on the border between the editor area and the memory area. Alternatively, one of the buttons in the Export group on the Import/Export tab can be used. (An appropriate file format will be selected by default.)

## Using color marking to filter out resources in the course of handling translation-memory data:

Color marking is performed using the Color drop-down list in the Markup group of the Home tab. When a color is selected from this list, all highlighted segments become marked with the selected color. A segment can only be marked with one color at a time and will always be marked in its entirety. (For convenience, the TU# field remains unmarked.) The Clear Markup option, which is also shown on the drop-down list, can be selected to clear any highlighted marked segments.

Marking-based filtering is performed using the Color drop-down list from the Marked Up group of the Filters and Checks tab. If any colors are selected from this list (multiple colors can be selected simultaneously), the editor will not display any segments not marked with these colors.

Using standard find-and-replace functions in the editor, with the option of using regular expressions available:

The user can activate the Search and Replace window by pressing either CTRL+F or the Search button in the Text Search group of the Home tab.

## Cleaning up resources by removing tags of various types (including the XML and RTF tags) as well as any superfluous spaces at the start and at the end of a given text:

The Clean drop-down list in the Text Cleaning group of the Home tab is used for this purpose. Selecting any of the items on the list executes the corresponding operation for all highlighted cells.

**Tags only** removes any angle bracket (< >) tags.

**Tags such as { }** remove any curly bracket or other corresponding tags.

**Trim first and last spaces** removes any unneeded spaces.

**Clear cells** clears the cells.

## Filtering resources using various criteria such as segment status and presence of particular text fragments within cell

Various elements of the Filters and Checks tab are used for this purpose:

- The **Clear** button resets the list of filtering criteria;

- The **Status** button group is used for displaying only new, modified or locked segments in the editor. Segments can be locked or unlocked using the Protection button group of the Home tab.

- The Marked Up element group: See the above description.

- The Search element group is used to filter away any segments that don't contain the specified text fragment. A specific segment field, selected by means of the Field drop-down list, will be searched for the fragment entered in the Text box. If the Contains button is used to start the filtering process, the editor will display every segment that contains the text within the appropriate field. If the Equals button is used, only the segment in which the field’s content is a complete match to the text will be shown;

- The Advanced element group: see below.

## Executing QA checks by filtering. Various methods of selection based on source-target comparison are available.

- The **Filter Checks** drop-down list from the Advanced group of the Filters and Checks tab is used. It contains the following elements:

- **Source = Target** displays only the segment in which the contents of the source and target fields match

- **Capitalization** displays only the segment in which the text in the source and target fields begins with different capitalization

- **Leading and trailing spaces** displays only the segments with different leading and trailing spaces in their source and target fields

- **Double spaces** displays only the segment in which the source and target fields contain different sets of double spaces

- **Digits and numbers** displays only the segment in which the source and target fields contain different sets of digits and numbers

- **Placeholders** displays only the segment in which the source and target fields contain different sets of placeholders (i.e., formatted printing sequences: %s, %d, %1, etc.)

- **Punctuation** displays only the segment in which the source and target fields differ in leading and trailing punctuation

- **Relative size** displays only the segment in which the source and target fields vary greatly in the volume of text they contain

- **Empty segments** displays only the segment in which either the source or the target field is empty

- **Partially translated** displays only the segments in which the target field partially matches the content of the source field, pointing to partial translation

- **Find duplicates** displays duplicate segments

– The check is performed for a single language pair, i.e., the source language and a particular target language selected from the **Ref.Pair** drop-down list.

## Splitting or merging translation memory files using several criteria, in batch mode.

The **Split & Merge** group of the Batch Tools tab is used:

- The **Split** button opens a dialog window that is used to split TBX/TMX files, and the source file is selected by means of the Browse button. The size of the resulting files is determined by segment count or by file size, depending on the user's requirement. The OK button is activated when the source file and splitting method are selected.

- The **Merge** button opens a dialog window used for merging a batch of TBX/TMX files. The source language of the resulting file is selected from the Source/Admin language drop-down list or set by entering a language code. The File List element group facilitates the addition of all TMX/TBX files in a particular folder to the list (Add TMX Dir, Add TBX Dir), the addition of arbitrary files or groups of files (Add File), the removal of files from the list one by one (Delete) or the clearing of the list (Clear). The OK button becomes active when a source language is set and at least one or more files are added to the list.

## Converting XLSX files into the TMX, TBX or XLF format using the batch mode

The **Converters** group of the Batch Tools tab is used. Each of the buttons (Convert to TMX, Convert to TBX, Convert to XLF) calls a dialog window in which the user will:

- Select a single XLSX file for conversion using the Browse button.

- Set the languages for the resulting multilingual file. Each language has to be selected from the Language drop-down list (or entered as a language code) and added to the list by means of the Add button.

- Set the source language by selecting it from the Primary language drop-down list or entering a language code.

- The OK button becomes active when a XLSX file is selected and at least two languages are added to the list.

Goldpan lets the user choose each of the resources required from various sources and then merge them into new translation-memory resource files as needed.