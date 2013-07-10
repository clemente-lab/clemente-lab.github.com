---
layout: page
permalink: /publications/index.html
title: Publications
headline: Recent Publications
tags: [publication, publications, publishing, paper, papers, articles]
publication-count: 10
---

Here's a list of the {{ page.publication-count }} most recent publications to
come out of the Clemente Lab. For a full list of publications, check out
[Google Scholar](http://scholar.google.com/citations?user=n3vpktQAAAAJ) or
[PubMed](http://www.ncbi.nlm.nih.gov/pubmed?term=Clemente%20JC%5BAuthor%5D&cmd=DetailsSearch).

<div id="recentPublications">
  <center>
  <img src="{{ site.url }}/images/load.gif" />
  </center>
</div>

<script> 
  // Creates a PubMed list for the Author, this string should be the search term used by PubMed
  pubmed.createList("Clemente%20JC[Author]")
    //Optional - Sets the max number of records to retrieve
    .setMax(10) // default = 10

    //Optional - Sets whether or not the abstract of an article should be retrieved
    .retrieveAbstract(true) // default = true
    //Optional - Sets whether or not the abstract of an article should be collapsible
    .collapsibleAbstract(true) // default = true
    //Optional - Sets whether or not the abstract of an article should be pre-expanded
    // this only has an effect if collapsibleAbstract = true
    .openedAbstract(false) // default = false

    //Optional - Sets whether or not the details of an article should be retrieved
    .retrieveDetails(true) // default = true
    //Optional - Sets whether or not the details of an article should be collapsible
    .collapsibleDetails(false) // default = false
    //Optional - Sets whether or not the details of an article should be pre-expanded
    // this only has an effect if collapsibleDetails = true
    .openedDetails(false) // default = true

    //Optional - Override the function used to expand an element.
    .overrideExpand(function(domElement) {
      domElement.style.display = "inline"; //default implementation
    })

    //Optional - Override the function used to collapse an element.
    .overrideCollapse(function(domElement) {
      domElement.style.display = "none"; //default implementation
    })

    //Required - Converts the data to HTML and inserts it into the element with the specified ID
    .bind("recentPublications");
</script>
