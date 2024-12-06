---
layout: default
---

Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Mammalian Basal Ganglia Consensus Cell Type Atlas 

The basal ganglia (BG) are a system of interconnected brain structures that play a crucial role in motor control, learning, behavior, and emotion. With approximately 200 million neurons in the human basal ganglia alone, these structures are involved in a wide range of neurological processes and are implicated in numerous disorders affecting human health, including Parkinson’s disease, Huntington’s disease, and substance abuse disorders. To further understand the complexity of the basal ganglia, researchers have historically classified its neurons into various types based on their cytoarchitecture, connectivity, molecular profile, and functional properties. Recent advancements in high-throughput transcriptomic profiling and machine learning have revolutionized our ability to systematically categorize these cell types within species and integrate the taxonomies across species. We present a unified taxonomy of the mammalian basal ganglia, providing unprecedented insights into the conserved and divergent features of this system across humans, macaques, marmosets, and mice. 

## Consensus Cell Type Nomenclature 

To unify the field’s understanding of basal ganglia cell types across species, efforts supported by the NIH BRAIN Initiative have initiated a comprehensive nomenclature system that synthesizes pre-existing literature describing cell type nomenclature with new cross-species transcriptomic data. This effort includes coordinated contributions from the Human and Mammalian Brain Atlas (HMBA) project in the BRAIN Initiative Cell Atlas Network (BICAN), and the Basal Ganglia AAV Toolbox project of the BRAIN Initiative Armamentarium for Precision Cell Access. This initiative integrates HMBA single-nucleus RNA sequencing (snRNA-seq) data from human, macaque, marmoset, and previously published mouse basal ganglia, with the goal of generating a consensus cell type taxonomy that can be widely adopted by the scientific community. By focusing on conserved marker genes and shared molecular profiles to supplement established names from the broader community, we have developed a standardized naming system that captures the evolutionary relationships and functional distinctions among basal ganglia cell types. The HMBA consensus basal ganglia taxonomy is designed to streamline communication, foster collaboration, and facilitate the development of novel research tools targeting specific cell types across multiple species. 

## Sample and Cell Type Metadata Collection 

To support the HMBA consensus cell type taxonomy, we have compiled extensive metadata providing detailed information associated with each identified cell type. These metadata include information on gene expression patterns and marker genes from snRNA-seq as well as synonymous names from existing literature, including Yao et al. 2023 and Siletti et al 2023. The metadata fields will be organized under an aligned taxonomy data format enabling integration with pre-existing tools such as CellxGene and Cell Annotation Platform.  

## Cell Type Taxonomies 

Our consensus basal ganglia cell type taxonomy is the result of iterative clustering and cross-species integration of transcriptomic data from single-nucleus 10x Genomics multiomic profiling. The taxonomy encompasses neurons from key structures within the basal ganglia, including the caudate (Ca), putamen (Pu), nucleus accumbens (NAc), the external and internal segments of the globus pallidus (GPe, GPi), subthalamic nucleus (STN), and substantia nigra (SN). By combining data from multiple primate and rodent species, we have developed a consensus taxonomy that highlights both conserved and species-specific cell types. We validate our taxonomy through marker gene expression analysis, comparison with previously published taxonomies, and self-projection, ensuring the accuracy and robustness of each level in the taxonomic hierarchy. 

## Data and Cell Type Mapping 

Here we provide an initial version of the HMBA basal ganglia consensus taxonomy annotated onto both human and macaque 10X multiome (RNA-seq) profiling. Within each Allen Institute Taxonomy (AIT) .h5ad object you will find components necessary for analysis, visualization and cell type mapping using various algorithms via scrattch.mapping or cell_type_mapper. 

The AIT .h5ad files are organized according to a schema: 

| Species        | File Format  | Size          | Data Download     | Annotation Sheet |
|:---------------|:-------------|:--------------|:------------------|:-----------------|
| Human          | AIT (.h5ad)  | 34GB          | AWS S3 URL        | Google Sheet 
| Macaque        | AIT (.h5ad)  | 25GB          | AWS S3 URL        | Google Sheet 
| Marmoset       | AIT (.h5ad)  | TBD           | Available in 2025 | Available in 2025
| Mouse          | AIT (.h5ad)  | TBD           | Available in 2025 | Available in 2025

Additional details about building and organizing Allen Institute Taxonomy (AIT) files can be found here: scrattch.taxonomy. 

For tutorials showcasing how to use AIT files easily with basic and MapMyCells algorithms, please visit our scrattch.mapping tutorial. 

## A Cell Type-Specific Enhancer Virus Tool Collection 

In collaboration with the BRAIN Armamentarium Consortium, we have developed an extensive collection of cell type-specific viral tools, designed to target and manipulate specific cell types identified in our cross-species integrated consensus BG taxonomy (Hunker, Wirthlin, et al. 2024). Using bulk or single nucleus ATAC-seq and multiomic data, we identify cell type-specific gene regulatory elements—particularly enhancers—linked to the cell types we identified through snRNA-seq. These efforts have culminated in a robust computational pipeline for identifying successful enhancers with a high degree of accuracy, the Cross-species Enhancer Ranking Pipeline (CERP). This pipeline allows us to identify and prioritize testing of the most promising candidate cell type enhancers for targeting homologous cell types across mammalian species. This viral tool collection comprises hundreds of enhancer adeno-associated virus (AAV) vectors, each with detailed brain expression analysis catalogues in the Genetic Tools Atlas (GTA). The most promising tools were also subjected to molecular validation. Additionally, we offer variants of these tools with enhancers optimized for stronger or more specific labeling, as well as variants delivering fluorescent proteins, channelrhodopsin variants, GCaMP variants, recombinases (Cre and Flp) to enable targeted experimental manipulation for functional studies. Many of these enhancer AAV vectors are already available through Addgene, with new tools continuously being added to the collection. These collective resources provide researchers with a powerful toolkit for targeting and studying the diverse cell types of the basal ganglia across multiple species to advance our understanding of BG function and dysfunction in health and disease. 

## Consensus cell types targeted for viral tool labeling

Cell type subclasses in BG regions are conserved between mouse, human, and non-human primates. Candidate enhancers were identified for the major BG cell subclasses using a novel computational pipeline (CERP). Additional CERP enhancers were selected to target other BG cell populations, including groups of cell types with regional enrichment, such as dorsal vs. ventral striatum. 

## Major cell types of basal ganglia targeted for viral tool labeling.

A major release of tools for labeling and manipulating MSNs (all, as well as D1 direct pathway and D2 indirect pathway subtypes) and interneurons (cholinergic, Sst-Chodl, and fast-spiking Pvalb-Pthlh subtypes) provides opportunities for experimental interrogation of striatal types with unprecedented specificity. Further details of tool design presented in Hunker, Wirthlin, et al. 2024, with most available now on Addgene. Tools for a dozen additional cell types of the striatum and small nuclei of the basal ganglia planned for release in 2025. 

## Related Resources 

This resource will facilitate deeper exploration into the diversity of basal ganglia cell types, providing insights into the molecular underpinnings of neurological disorders and the evolutionary pathways that have shaped these critical brain structures. 

This page aims to serve as a gateway for researchers to access and explore our consensus basal ganglia cell type taxonomy. Through this resource, we hope to advance the understanding of basal ganglia function, facilitate the development of targeted therapies, and contribute to the broader field of comparative neurobiology. We encourage users to explore complementary efforts from both internal and outside collaborators.  

BRAIN Armamentarium Collection of viral tools to target BG cell types 

Cross-species Enhancer Ranking Pipeline (CERP) - Identify candidate enhancers in regions of open chromatin using single nucleus ATAC-seq data sets. Prioritize candidate enhancers based on conserved cell type-specific chromatin accessibility between macaque and mouse using ranking modules such as PeakRankR. 

Supported by the NIH BRAIN Initiative Armamentarium grant UF1MH128339 and Cell Atlas Network grant UM1MH130981. 

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```