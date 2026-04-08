
# Seri verbs 
This is a collection of verb paradigms in Seri, conforming to the [Paralex ](https://www.paralex-standard.org) standard. The metadata conforms to the [frictionless](https://frictionlessdata.io/) standard. Datafiles are encoded as `csv` files.

The dataset is is licensed under [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/?ref=chooser-v1)

NOTE: THIS DATASET IS UNDER CONSTRUCTION AND MAY NOT BE ACCURATE.

## Citation

TO ADD

## Contact us

TO ADD

## Sources

The primary source of this data is Moser and Marlett (2010):

Moser, M. B., & Marlett, S. A. 2010. *Comcáac quih yaza quih hant ihíip hac: Diccionario seri-español-inglés con índices español - seri, inglés -seriycon gramática* (2nd ed.). Editorial UniSon / Plaza y Valdés Editores. https://www.sil.org/system/files/reapdata/10/33/81/103381195691201622442706606620865373126/sei_diccionario_ed2.pdf

(Add reference for the grammar too)

## How the data was prepared

This data was derived automatically from electronic dictionary data. While we have made reasonable efforts to validate the output manually, some errors may remain. In particular:
- the `gloss` given in `lexemes.csv` has been automatically translated from Spanish, and may not be fully accurate. This data should not be relied on for semantic information.
- Some lexemes listed in `lexemes.csv` could not be parsed, and therefore do not appear in `forms.csv`
- Where multiple paradigms are listed in the dictionary for a single headword, these have been interpreted as multiple homophonous lexemes for the purposes of this data. Homophonous lexemes are indicated with numerical extensions in the `lexeme_id` field, e.g. `"quip_2"`.

## Notes on the analysis

### Orthography
- The forms in `forms.csv` are given in a conventional transcription ('practical orthography') in the column `orth_form`, and in an IPA based transcription in the column `phon_form`. 
- Individual segments are separated by spaces. 
- Correspondences between graphemes and phonemes are given in the table `graphemes.csv`. 
- The phonemes are described in more detail in `sounds.csv`.
- Some orthographic forms contain spaces. This reflects orthographic convention, but they are morphologically a single inflected word (i.e. these are not periphrastic constructions)

### Phonology
- The forms listed in the `phon_form` field of `forms.csv`  are phonological forms, rather than phonetic.
- Stress is not currently indicated. We hope to change this in a future version of the dataset.
- TO ADD: epenthetic i- in some forms not indicated.

### Morphosyntax

#### Paradigm structure
- For the vast majority of verbs, only the subparadigm of the realis-t.pos.3 is listed. This is sufficient to show how forms of different number values (for person and event number) relate to each other.
- We give a broader range of forms, illustrative of the whole paradigms, for the sample of verbs listed in (add references to back of grammar + dictionary).
- ADD SOMETHING ON VOICE 

#### Distributives
- Where three singular forms are listed, one of which has the suffix -tim/-im, we analyse the first form listed as having neutral event number, and of the remaining two forms, we analyse the form in -tim/im as multiple and the other as distributive
- Where a distributive is not explicitly listed, we assume the distributive is syncretic with the multiple
- (Add references)

#### Omitted features and values
- There are additional 1sg emphatic forms, which are unrelated to the emphatic realis mood (`real-emph`). We do not list these.
- We do not give indefinite forms (unmarked for subject person)
- We don't include object marking. The 3rd person transitive forms encode a 3rd person object (the i- prefix represents 3>3). other forms implicitly have 3rd person objects.  

