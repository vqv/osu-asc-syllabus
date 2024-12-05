# The Ohio State University ASC Distance Learning Syllabus Format

This is a Quarto extension for creating syllabi that closely 
match the [ASC Distance Learning Syllabus Template](https://go.osu.edu/ascsyllabustemplate). 
The ASC Distance Learning Syllabus Template is a Word document that includes 
additional content beyond the standard ASC syllabus. So this extension 
can also be used for creating syllabi for in-person or hybrid courses.


## Installing

```bash
quarto use template vqv/osu-syllabus
```

This will install the extension and create an example qmd file that you can 
use as a starting place for your syllabus.

## Using

All of the 
[ASC syllabus elements](https://asccas.osu.edu/submission/development/submission-materials/syllabus-elements), 
both required and optional, are included in the example file. The 
`## Academic policies` section includes the standard ASC policies 
in the `asc-dl-academic-policies.qmd` file provided by the extension. 
Be careful with relative paths if you modify the example. 

The extension provides two custom formats: `osu-syllabus-docx` and 
`osu-syllabus-html`. The former is used to create a Word document that 
closely matches the template, while the latter is used to create an HTML that 
can be uploaded to CarmenCanvas. I recommend using Quarto's 
[conditional content](https://quarto.org/docs/authoring/conditional.html) 
feature, particularly `.content-visible unless-format="docx"`, to exclude 
 sections that you may not want to include in the HTML that you upload 
 to CarmenCanvas.

**Note**: I created this extension for my own teaching in the Department of 
Statistics, so you may need to modify the heading in 
`_extensions/osu-asc-syllabus/reference.docx` to match your 
unit's name.

## Example

*TODO*: The next version of the extension will include an examples for 
generating the schedule programmatically from a CSV file. 
