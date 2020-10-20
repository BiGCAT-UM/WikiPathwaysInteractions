### Interactions

ShEx for Interactions

```turtle
@prefix wp:    <http://vocabularies.wikipathways.org/wp#> .
@prefix dcterms: <http://purl.org/dc/terms/> .

<http://rdf.wikipathways.org/Pathway/WP4806_r110852/WP/Interaction/ae20c>
        a                 wp:DirectedInteraction , wp:Interaction ;
        dcterms:isPartOf  <http://identifiers.org/wikipathways/WP4806_r110852> ;
        wp:isAbout        <http://rdf.wikipathways.org/Pathway/WP4806_r110852/Interaction/ae20c> ;
        wp:participants   <http://identifiers.org/ncbigene/2549> , <http://identifiers.org/ensembl/ENSG00000146648> ;
        wp:source         <http://identifiers.org/ensembl/ENSG00000146648> ;
        wp:target         <http://identifiers.org/ncbigene/2549> .
```

ShEx for a general interaction:

```shex
PREFIX dc: <http://purl.org/dc/elements/1.1/>
PREFIX wp: <http://vocabularies.wikipathways.org/wp#>

<interaction> {
  wp:participants   IRI {1,} 
}
```
ShEx for directed interactions:

```shex
PREFIX dc: <http://purl.org/dc/elements/1.1/>
PREFIX wp: <http://vocabularies.wikipathways.org/wp#>

<interaction> {
  wp:participants   IRI {2,} ;
  wp:source         IRI ;
  wp:target         IRI
}
```
