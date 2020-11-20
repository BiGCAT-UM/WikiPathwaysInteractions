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

## Testing

Copy the turtle into `interaction.ttl` and the shape expression into `interaction.shex` and http://rdf.wikipathways.org/Pathway/WP4806_r110852/WP/Interaction/ae20c
`directed_interaction.shex` and then run:

```shell
npm install --save shex
./node_modules/shex/bin/validate -d interaction.ttl -x interaction.shex -n http://rdf.wikipathways.org/Pathway/WP4806_r110852/WP/Interaction/ae20c
./node_modules/shex/bin/validate -d interaction.ttl -x directed_interaction.shex -n http://rdf.wikipathways.org/Pathway/WP4806_r110852/WP/Interaction/ae20c
```


### BINDINGS 
```turtle
@prefix wp:    <http://vocabularies.wikipathways.org/wp#> .
@prefix dcterms: <http://purl.org/dc/terms/> .
<http://rdf.wikipathways.org/Pathway/WP1434_r94913/ComplexBinding/f69ea>
        a                 wp:ComplexBinding , wp:Binding , wp:Interaction ;
        dcterms:isPartOf  <http://identifiers.org/wikipathways/WP1434_r94913> ;
        wp:isAbout        "http://rdf.wikipathways.org/Pathway/WP1434_r94913/Group/f69ea" ;
        wp:participants   <http://identifiers.org/ncbigene/3690> , <http://identifiers.org/ncbigene/3685> , <http://rdf.wikipathways.org/Pathway/WP1434_r94913/Complex/f69ea> .
```

ShEX for Binding interactions

```shex
PREFIX dc: <http://purl.org/dc/elements/1.1/>
PREFIX wp: <http://vocabularies.wikipathways.org/wp#>

<interaction> {
  wp:participants   IRI {1,} 
}
```

ShEx for Complex Binding interactions

```shex
PREFIX dc: <http://purl.org/dc/elements/1.1/>
PREFIX wp: <http://vocabularies.wikipathways.org/wp#>

<interaction> {
  wp:participants   IRI {1,} 
}
```

### CONVERSIONS 
```turtle
@prefix wp:    <http://vocabularies.wikipathways.org/wp#> .
@prefix dcterms: <http://purl.org/dc/terms/> .
<http://rdf.wikipathways.org/Pathway/WP1946_r96397/WP/Interaction/af536>
        a                 wp:Conversion , wp:DirectedInteraction , wp:Interaction ;
        dcterms:isPartOf  <http://identifiers.org/wikipathways/WP1946_r96397> ;
        wp:isAbout        <http://rdf.wikipathways.org/Pathway/WP1946_r96397/Interaction/af536> ;
        wp:participants   <http://identifiers.org/hmdb/HMDB0001401> , <http://identifiers.org/chebi/CHEBI:28087> ;
        wp:source         <http://identifiers.org/chebi/CHEBI:28087> ;
        wp:target         <http://identifiers.org/hmdb/HMDB0001401> .

```
ShEx for Conversion interactions:

```shex
PREFIX dc: <http://purl.org/dc/elements/1.1/>
PREFIX wp: <http://vocabularies.wikipathways.org/wp#>

<interaction> {
  wp:participants   IRI {2,} ;
  wp:source         IRI ;
  wp:target         IRI
}
```

### INHIBITIONS 
```turtle
@prefix wp:    <http://vocabularies.wikipathways.org/wp#> .
@prefix dcterms: <http://purl.org/dc/terms/> .
<http://rdf.wikipathways.org/Pathway/WP1471_r94755/WP/Interaction/a2d4f>
        a                 wp:Inhibition , wp:DirectedInteraction , wp:Interaction ;
        dcterms:isPartOf  <http://identifiers.org/wikipathways/WP1471_r94755> ;
        wp:isAbout        <http://rdf.wikipathways.org/Pathway/WP1471_r94755/Interaction/a2d4f> ;
        wp:participants   <http://identifiers.org/wikipathways/WP107> , <http://identifiers.org/ensembl/ENSG00000187840> ;
        wp:source         <http://identifiers.org/ensembl/ENSG00000187840> ;
        wp:target         <http://identifiers.org/wikipathways/WP107> .

```
ShEx for Inhibition interactions:

```shex
PREFIX dc: <http://purl.org/dc/elements/1.1/>
PREFIX wp: <http://vocabularies.wikipathways.org/wp#>

<interaction> {
  wp:participants   IRI {2,} ;
  wp:source         IRI ;
  wp:target         IRI
}
```
### CATALYSIS   
```turtle
@prefix wp:    <http://vocabularies.wikipathways.org/wp#> .
@prefix dcterms: <http://purl.org/dc/terms/> .
<http://rdf.wikipathways.org/Pathway/WP1946_r96397/WP/Interaction/a8b0e>
        a                 wp:Catalysis , wp:DirectedInteraction , wp:Interaction ;
        dcterms:isPartOf  <http://identifiers.org/wikipathways/WP1946_r96397> ;
        wp:isAbout        <http://rdf.wikipathways.org/Pathway/WP1946_r96397/Interaction/a8b0e> ;
        wp:participants   <http://identifiers.org/uniprot/ALDOA> , <http://rdf.wikipathways.org/Pathway/WP1946_r96397/WP/Interaction/id4f52ff91> ;
        wp:source         <http://identifiers.org/uniprot/ALDOA> ;
        wp:target         <http://rdf.wikipathways.org/Pathway/WP1946_r96397/WP/Interaction/id4f52ff91> .

```
ShEx for Catalysis interactions:

```shex
PREFIX dc: <http://purl.org/dc/elements/1.1/>
PREFIX wp: <http://vocabularies.wikipathways.org/wp#>

<interaction> {
  wp:participants   IRI {2,} ;
  wp:source         IRI ;
  wp:target         IRI
}
```

### STIMULATIONS   
```turtle
@prefix wp:    <http://vocabularies.wikipathways.org/wp#> .
@prefix dcterms: <http://purl.org/dc/terms/> .
<http://rdf.wikipathways.org/Pathway/WP3965_r96169/WP/Interaction/id5d32d209>
        a                 wp:Stimulation , wp:DirectedInteraction , wp:Interaction ;
        dcterms:isPartOf  <http://identifiers.org/wikipathways/WP3965_r96169> ;
        wp:isAbout        <http://rdf.wikipathways.org/Pathway/WP3965_r96169/Interaction/id5d32d209> ;
        wp:participants   <http://identifiers.org/ensembl/ENSG00000177666> , <http://identifiers.org/ensembl/ENSG00000011198> ;
        wp:source         <http://identifiers.org/ensembl/ENSG00000011198> ;
        wp:target         <http://identifiers.org/ensembl/ENSG00000177666> .

```
ShEx for Stimulation interactions:

```shex
PREFIX dc: <http://purl.org/dc/elements/1.1/>
PREFIX wp: <http://vocabularies.wikipathways.org/wp#>

<interaction> {
  wp:participants   IRI {2,} ;
  wp:source         IRI ;
  wp:target         IRI
}
```

### TRANSCRIPTION-TRANSLATIONS  
```turtle
@prefix wp:    <http://vocabularies.wikipathways.org/wp#> .
@prefix dcterms: <http://purl.org/dc/terms/> .
<http://rdf.wikipathways.org/Pathway/WP3982_r96401/WP/Interaction/a5ddb>
        a                 wp:TranscriptionTranslation , wp:DirectedInteraction , wp:Interaction ;
        dcterms:isPartOf  <http://identifiers.org/wikipathways/WP3982_r96401> ;
        wp:isAbout        <http://rdf.wikipathways.org/Pathway/WP3982_r96401/Interaction/a5ddb> ;
        wp:participants   <http://identifiers.org/ensembl/ENSG00000149547> , <http://identifiers.org/chebi/CHEBI:16991> ;
        wp:source         <http://identifiers.org/chebi/CHEBI:16991> ;
        wp:target         <http://identifiers.org/ensembl/ENSG00000149547> .

```
ShEx for TranscriptionTranslation interactions:

```shex
PREFIX dc: <http://purl.org/dc/elements/1.1/>
PREFIX wp: <http://vocabularies.wikipathways.org/wp#>

<interaction> {
  wp:participants   IRI {2,} ;
  wp:source         IRI ;
  wp:target         IRI
}
```
