
<!-- README.md is generated from README.Rmd. Please edit that file -->

## Source code for the [MAGA Keyword Screener](https://jhelvy.github.io/magaScreener/) app

This tool allows you to analyze documents for MAGA-targeted
[keywords](https://github.com/jhelvy/magaScreener/blob/main/keywords.csv).
You can also upload your own CSV file of keywords. It is intended to be
used to help identify words that might get screened by an entity (e.g.,
the federal government) so you can modify your language accordingly.
Just upload a document, and the app will count occurrences of the
keywords.

Here’s a quick visual demo:

<center>
<img src="demo.gif" width=600>
</center>

**Supported File Types**:

- Word Documents: .docx, .doc
- PDF Files: .pdf
- Text Files: .txt
- Spreadsheets: .csv, .xlsx
- Web Documents: .html, .htm, .xml
- Other: .rtf, .json

### How It Works

The analyzer extracts text from your document and searches for keywords
from our predefined list. It then counts how many times each keyword
appears in your document. That’s all - it’s pretty simple.

All of the calculations run locally in your web browser using [web
assembly](https://webassembly.org/). Whatever you upload isn’t stored or
sent anywhere for processing, so you can upload even sensitive documents
without worry. You can also [run it locally](#locally-running-the-app)
on your computer if you want.

This site was built entirely using open-source tools. It uses the
[Quarto](https://quarto.org/) publishing system to build the website,
the [R programming language](https://www.r-project.org/) for logic, and
the [shiny](https://shiny.posit.co/) web application framework to
implement the R code, leveraging
[shinylive](https://quarto.org/docs/blog/posts/2022-10-25-shinylive-extension/)
Quarto extension to run the whole thing in the browser as a static web
page (thanks to [@coatless](https://github.com/coatless) for posting
such a great
[tutorial](https://github.com/coatless-quarto/r-shinylive-demo) on how
to set this up). The site itself is hosted on GitHub pages, and the
source code can be found at <https://github.com/jhelvy/magaScreener>.

### Locally Running the App

You can run the app on your local machine without even being connected
to the internet. To do so, follow these steps:

**Install stuff**

1.  Install [R](https://cloud.r-project.org/)
2.  Install [RStudio
    Desktop](https://posit.co/download/rstudio-desktop/)
3.  Install [Quarto](https://quarto.org/docs/get-started/)

**Download and run the app**

Once everything is installed, download the [source
code](https://github.com/jhelvy/magaScreener/archive/refs/heads/main.zip),
then unzip the file and open the `"magaScreener.Rproj"` file. This
should open RStudio.

Once open, click on the `"index.qmd"` file, then click the “render”
button at the top of the RStudio application (it has a little blue arrow
next to it). This should open a web browser from where you can then use
the application.

Alternatively you can click on the `"Terminal"` window and run the
following command:

``` r
quarto preview
```

### Keywords List

The analyzer searches for the following keywords:

|                            |
|:---------------------------|
| accessible                 |
| activism                   |
| activists                  |
| advocacy                   |
| advocate                   |
| advocates                  |
| affirming care             |
| all-inclusive              |
| allyship                   |
| anti-racism                |
| antiracist                 |
| assigned at birth          |
| assigned female at birth   |
| assigned male at birth     |
| assigned male              |
| assigned female            |
| at risk                    |
| barrier                    |
| barriers                   |
| belong                     |
| bias                       |
| biased                     |
| biased toward              |
| biases                     |
| biases towards             |
| biologically female        |
| biologically male          |
| BIPOC                      |
| Black                      |
| breastfeed                 |
| breastfeed + people        |
| breastfeed + person        |
| chestfeed                  |
| chestfeed + people         |
| chestfeed + person         |
| clean energy               |
| climate crisis             |
| climate science            |
| commercial sex worker      |
| community diversity        |
| community equity           |
| confirmation bias          |
| cultural competence        |
| cultural differences       |
| cultural heritage          |
| cultural sensitivity       |
| culturally appropriate     |
| culturally responsive      |
| DEI                        |
| DEIA                       |
| DEIAB                      |
| DEIJ                       |
| disabilities               |
| disability                 |
| discriminated              |
| discrimination             |
| discriminatory             |
| disparity                  |
| diverse                    |
| diverse backgrounds        |
| diverse communities        |
| diverse community          |
| diverse group              |
| diverse groups             |
| diversified                |
| diversify                  |
| diversifying               |
| diversity                  |
| enhance the diversity      |
| enhancing diversity        |
| environmental quality      |
| equal opportunity          |
| equality                   |
| equitable                  |
| equitableness              |
| equity                     |
| ethnicity                  |
| excluded                   |
| exclusion                  |
| expression                 |
| female                     |
| females                    |
| feminism                   |
| fostering inclusivity      |
| GBV                        |
| gender                     |
| gender based               |
| gender based violence      |
| gender diversity           |
| gender identity            |
| gender ideology            |
| gender-affirming care      |
| genders                    |
| Gulf of Mexico             |
| hate speech                |
| health disparity           |
| health equity              |
| hispanic minority          |
| historically               |
| identity                   |
| immigrants                 |
| implicit bias              |
| implicit biases            |
| inclusion                  |
| inclusive                  |
| inclusive leadership       |
| inclusiveness              |
| inclusivity                |
| increase diversity         |
| increase the diversity     |
| indigenous community       |
| inequalities               |
| inequality                 |
| inequitable                |
| inequities                 |
| inequity                   |
| injustice                  |
| institutional              |
| intersectional             |
| intersectionality          |
| key groups                 |
| key people                 |
| key populations            |
| Latinx                     |
| LGBT                       |
| LGBTQ                      |
| marginalize                |
| marginalized               |
| men who have sex with men  |
| mental health              |
| minorities                 |
| minority                   |
| most risk                  |
| MSM                        |
| multicultural              |
| Mx                         |
| Native American            |
| non-binary                 |
| nonbinary                  |
| oppression                 |
| oppressive                 |
| orientation                |
| uterus                     |
| people + uterus            |
| people-centered care       |
| person-centered            |
| person-centered care       |
| polarization               |
| political                  |
| pollution                  |
| pregnant people            |
| pregnant person            |
| pregnant persons           |
| prejudice                  |
| privilege                  |
| privileges                 |
| promote diversity          |
| promoting diversity        |
| pronoun                    |
| pronouns                   |
| prostitute                 |
| race                       |
| race and ethnicity         |
| racial                     |
| racial diversity           |
| racial identity            |
| racial inequality          |
| racial justice             |
| racially                   |
| racism                     |
| segregation                |
| sense of belonging         |
| sex                        |
| sexual preferences         |
| sexuality                  |
| social justice             |
| sociocultural              |
| socioeconomic              |
| status                     |
| stereotype                 |
| stereotypes                |
| systemic                   |
| systemically               |
| they/them                  |
| trans                      |
| transgender                |
| transsexual                |
| trauma                     |
| traumatic                  |
| tribal                     |
| unconscious bias           |
| underappreciated           |
| underprivileged            |
| underrepresentation        |
| underrepresented           |
| underserved                |
| undervalued                |
| victim                     |
| victims                    |
| vulnerable populations     |
| woke                       |
| women                      |
| women and underrepresented |
