# LanguagesGallery
**Lingualibre Languages Gallery** is a VueJS searchable gallery of Lingualibre languages, with relevant statistics, call to action, and access to download our open licence datasets.

## Why a language gallery ?
The *Lingualibre Languages Gallery* is the fruits of 2 years of periodic research and developement. It started in late 2021, with the writing of [Help:SPARQL](https://lingualibre.org/wiki/Help:SPARQL) which aimed to explore per language statistics, including on gender coverage and geographic distribution. Advanced SPARQL queries confirmed our suspicions, the major geographic and gender biaises found raised the need for an human friendly, searchable *Languages gallery* able to communicate those findings to both the general public and Wikimedia policies makers. 

## Solution
The language gallery stands upon data consolidation pipeline and daily publication systems, the [Sparql2data](https://github.com/hugolpz/Sparql2data) bash script. Using refined SPARQL queries, both Lingualibre and Wikidata's data are fetched daily, their JSON responses saved in persistant files and served online. Responsive HTML/CSS code was adapted from Common Voice Project, with whom further collaboration would be welcome.

The whole does the job elegantly, providing per language key metrics, with a search function, call to action, datasets download and sharable links.

## Design
<img src="https://github.com/hugolpz/LanguagesGallery/assets/1420189/3a81cdbc-ccdd-4f98-8896-64a4d7d0cca3" alt="Image" width="300" align="right">
This page presents Lingualibre.org's statistics on a per languages basis with:

- Language name (Wikidata)
- Number of native speakers worldwide. (Wikidata)
- Speakers : number of Lingualibre speakers, aka voices. (Lingualibre)
- Gender split : number of females, other (non-binary and undefined), males voices. (Lingualibre)
- Unique words vs recordings ratio. (Lingualibre)
- Recordings gender split: number of females, other (non-binary and undefined), males recordings. (Lingualibre)
- Contribute button: points to our online rapid recording studio.
- Download button: download access to all open licence audios in this language.

![Screenshot from 2023-06-04 21-59-20](https://github.com/hugolpz/LanguagesGallery/assets/1420189/c26bc81e-299c-4126-acdc-95d06c3052f4)
<br clear=all>

## Advanced features
- Search and filter by English or native language name
- Share a filtered url by appending `?search=YourSearch` to the url

## Datasets reuse
Each language's card has a download button to get a zip of all our open licence files. Their filenames should be used to point to the rightful Wikimedia file page, containing the file's licence.

## Contribute
This Single Page Web Application works with:
- HTML
- CSS
- VueJS

## Credits
Sorted by involvement: Yug, Elfix, VIGNERON, Poslovitch, Envel.

## License
See [index.html](./index.html)'s footer and [LICENSE MPL](./LICENSE).
