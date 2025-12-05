[![GloBI Review by Elton](../../actions/workflows/review.yml/badge.svg)](../../actions/workflows/review.yml) [![GloBI](https://api.globalbioticinteractions.org/interaction.svg?accordingTo=globi:globalbioticinteractions/fungaltraits&refutes=true&refutes=false)](https://globalbioticinteractions.org/?accordingTo=globi:globalbioticinteractions/fungaltraits)

Configuration to help Global Biotic Interactions (GloBI, https://globalbioticinteractions.org) index: 

Põlme, S., Abarenkov, K., Henrik Nilsson, R. et al. FungalTraits: a user-friendly traits database of fungi and fungus-like stramenopiles. Fungal Diversity 105, 1–16 (2020). https://doi.org/10.1007/s13225-020-00466-2

or

```bibtex
 @article{P_lme_2020, title={FungalTraits: a user-friendly traits database of fungi and fungus-like stramenopiles}, volume={105}, ISSN={1878-9129}, url={http://dx.doi.org/10.1007/s13225-020-00466-2}, DOI={10.1007/s13225-020-00466-2}, number={1}, journal={Fungal Diversity}, publisher={Springer Science and Business Media LLC}, author={Põlme, Sergei and Abarenkov, Kessy and Henrik Nilsson, R. and Lindahl, Björn D. and Clemmensen, Karina Engelbrecht and Kauserud, Havard and Nguyen, Nhu and Kjøller, Rasmus and Bates, Scott T. and Baldrian, Petr and Frøslev, Tobias Guldberg and Adojaan, Kristjan and Vizzini, Alfredo and Suija, Ave and Pfister, Donald and Baral, Hans-Otto and Järv, Helle and Madrid, Hugo and Nordén, Jenni and Liu, Jian-Kui and Pawlowska, Julia and Põldmaa, Kadri and Pärtel, Kadri and Runnel, Kadri and Hansen, Karen and Larsson, Karl-Henrik and Hyde, Kevin David and Sandoval-Denis, Marcelo and Smith, Matthew E. and Toome-Heller, Merje and Wijayawardene, Nalin N. and Menolli, Nelson and Reynolds, Nicole K. and Drenkhan, Rein and Maharachchikumbura, Sajeewa S. N. and Gibertoni, Tatiana B. and Læssøe, Thomas and Davis, William and Tokarev, Yuri and Corrales, Adriana and Soares, Adriene Mayra and Agan, Ahto and Machado, Alexandre Reis and Argüelles-Moyao, Andrés and Detheridge, Andrew and de Meiras-Ottoni, Angelina and Verbeken, Annemieke and Dutta, Arun Kumar and Cui, Bao-Kai and Pradeep, C. K. and Marín, César and Stanton, Daniel and Gohar, Daniyal and Wanasinghe, Dhanushka N. and Otsing, Eveli and Aslani, Farzad and Griffith, Gareth W. and Lumbsch, Thorsten H. and Grossart, Hans-Peter and Masigol, Hossein and Timling, Ina and Hiiesalu, Inga and Oja, Jane and Kupagme, John Y. and Geml, József and Alvarez-Manjarrez, Julieta and Ilves, Kai and Loit, Kaire and Adamson, Kalev and Nara, Kazuhide and Küngas, Kati and Rojas-Jimenez, Keilor and Bitenieks, Krišs and Irinyi, Laszlo and Nagy, László G. and Soonvald, Liina and Zhou, Li-Wei and Wagner, Lysett and Aime, M. Catherine and Öpik, Maarja and Mujica, María Isabel and Metsoja, Martin and Ryberg, Martin and Vasar, Martti and Murata, Masao and Nelsen, Matthew P. and Cleary, Michelle and Samarakoon, Milan C. and Doilom, Mingkwan and Bahram, Mohammad and Hagh-Doust, Niloufar and Dulya, Olesya and Johnston, Peter and Kohout, Petr and Chen, Qian and Tian, Qing and Nandi, Rajasree and Amiri, Rasekh and Perera, Rekhani Hansika and dos Santos Chikowski, Renata and Mendes-Alvarenga, Renato L. and Garibay-Orijel, Roberto and Gielen, Robin and Phookamsak, Rungtiwa and Jayawardena, Ruvishika S. and Rahimlou, Saleh and Karunarathna, Samantha C. and Tibpromma, Saowaluck and Brown, Shawn P. and Sepp, Siim-Kaarel and Mundra, Sunil and Luo, Zhu-Hua and Bose, Tanay and Vahter, Tanel and Netherway, Tarquin and Yang, Teng and May, Tom and Varga, Torda and Li, Wei and Coimbra, Victor Rafael Matos and de Oliveira, Virton Rodrigo Targino and de Lima, Vitor Xavier and Mikryukov, Vladimir S. and Lu, Yongzhong and Matsuda, Yosuke and Miyamoto, Yumiko and Kõljalg, Urmas and Tedersoo, Leho}, year={2020}, month=nov, pages={1–16} }
```

## Files

| name | description | origin |
| --- | --- | --- |
| polme2020-s1-fungal-traits-genera.csv | comma-separated values of content of "data" sheet in Põlme et al. 2020 Table S1. Traits of genera. Supplementary material 4 (XLSX 967 kb)| see #fungal-traits-of-genera
| polme2020-s1-fungal-traits-genera.tsv | idem, but in tab-separated values format | idem
| polme2020-s2-fungal-traits-sequences.csv.gz | comma-separated values of Põlme et al. 2020 Table S2. Traits of sequences. Supplementary material 5 (XLSX 56685 kb) | see #fungal-traits-of-sequences
| polme2020-s2-fungal-traits-sequences.tsv.gz | idem, but in tab-separated values format | idem |
| biblio.bib | contains citation of Põlme et al. 2020 in bibtex | manually entered to aid GloBI data review |
| globi.json | contains configuration to help GloBI index Põlme et al. 2020 tables S1 and S2 | automatically generated using ```elton init``` then manually configured |
| interaction_types_mapping.csv | translation table to relate terms in Põlme et al. 2020 to equivalent terms in the Relation Ontology | manually curated |
| README.md | this file | automatically generated using ```elton init``` then manually edited |


To help aid machine-readability of the data appendices of Põlme et al. 2020, snapshots of three data appendices were made using:

```
preston track --algo md5 \
 https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM5_ESM.xlsx \
 https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM6_ESM.xlsx \
https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM4_ESM.xlsx
```

## Fungal Traits of Sequences

then, the file ```https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM5_ESM.xlsx``` with fingerprint ```hash://md5/72e125ee5986aa61f587daa41d463b35``` and referred to as ```Table S2. Traits of sequences. Supplementary material 5 (XLSX 56685 kb)``` was transformed in a gzip compressed tab-separated values file ```fungal-traits-sequences.tsv.gz``` using:

```bash
preston cat hash://md5/147d1eed43249ce2ac1f8b9fb63765b1 \
 | grep hasVersion \
 | grep "13225_2020_466_MOESM5_ESM.xlsx" \
 | preston xlsx-stream \
 | mlr --ijsonl --otsvlite cat \
 | gzip \
 > fungal-traits-sequences.tsv.gz
```
and 

```bash
preston cat hash://md5/147d1eed43249ce2ac1f8b9fb63765b1 \
 | grep hasVersion \
 | grep "13225_2020_466_MOESM5_ESM.xlsx" \
 | preston xlsx-stream \
 | mlr --ijsonl --ocsv cat \
 | gzip \
 > fungal-traits-sequences.csv.gz
```

With first record being:

```
http://www.w3.org/ns/prov#wasDerivedFrom     line:xlsx:hash://md5/72e125ee5986aa61f587daa41d463b35!/fungal%20sequnce%20traits%20COMPLETED!/L2
http://purl.org/dc/elements/1.1/format       application/vnd.openxmlformats-officedocument.spreadsheetml.sheet
Sampling_area_Project                        Morris,M.H., Perez-Perez,M.A., Smith,M.E. and Bledsoe,C.S.; Multiple species of ectomycorrhizal fungi are frequently detected on individual oak root tips in a tropical cloud forest; Mycorrhiza 18 (8), 375-383 (2008)
updated_study_DOI                            10.1007/s00572-008-0186-1
Sequence_ID                                  EU563475
Sequence_quality                             null
INSD_original_data_Lineage                   Eukaryota; Fungi; Dikarya; Ascomycota; Pezizomycotina; Pezizomycetes; Pezizales; environmental samples
INSD_original_data_Organism                  uncultured Pezizales
Identification_Taxon_name                    null
Related_source_content_type                  Material Sample
Related_source_identifier                    Quercus root sample
INSD_original_data_Source                    ectomycorrhizal root tip
INSD_original_data_Tissue_type               null
DNA_isolation_source                         ectomycorrhiza
Culture_source                               null
Animal/human_tissue                          null
Guild                                        null
Growth_form                                  filamentous_mycelium
Ectomycorrhiza_exploration_type              null
Ericoid_mycorrhiza_formation                 null
Endophytic_interaction_capability            null
Plant/fungal_pathogenic_capacity             null
Animal/human_biotrophic_interaction_capacity null
Interactions                                 Quercus
Interacting_taxon                            Quercus crassifolia
Co-occurring_taxa                            Quercus laurina, Q. castanea
INSD_original_data_Clone                     M104C
INSD_original_data_Isolate                   null
INSD_original_data_Culture_collection        null
Strain                                       null
Specimen_voucher                             null
Type_status                                  null
Sampling_area_Locality_text                  Mexico: Huizteco
Sampling_area_Name                           Mexico
Country                                      Mexico
Sampling_area_State/Province                 Guerrero
Locality_text                                Huizteco Park, c. 4.5 km north of Taxco
Latitude                                     18.6
Longitude                                    -99.6
Measurement__Elevation_max                   null
Measurement__Elevation_min                   2500
Altitude                                     2500
Measurement__Depth_min                       null
Measurement__Depth_max                       null
Depth                                        null
Habitat_Description                          Subtropical montane Quercus forest
Habitat_IUCN_habitat_type                    13 - Marine Coastal/Supratidal
Biome                                        forest: tropical broadleaf forest biome
INSD_UNITE_remarks                           null
Remarks                                      null
Annotator                                    Adriana Corrales
column49                                     null
column50                                     null
PLUTOF_ID                                    42981
```

Note that the first two columns (i.e., ```http://www.w3.org/ns/prov#wasDerivedFrom```, ```http://purl.org/dc/elements/1.1/format```) document the sheet and excel sheet row number the csv row was derived from, as well as the original file type of the data source. In this case, the file type was always ```application/vnd.openxmlformats-officedocument.spreadsheetml.sheet``` which is the more formal mimetype of the commonly referred file type XLSX used by spreadsheet programs. 

## Fungal Traits for Genera

Similarly, the associated fungal traits appendix for genera was converted to tsv/csv using  

```
preston cat hash://md5/147d1eed43249ce2ac1f8b9fb63765b1 \
 | grep hasVersion \
 | grep "13225_2020_466_MOESM4_ESM.xlsx" \
 | preston xlsx-stream \
 | grep 'line:xlsx:hash://md5/9168998921adc01b1cf63d9cdca8342e!/data!/L' \
 | mlr --ijsonl --otsvlite cat \
 > fungal-traits-genera.tsv 
```

and 

```
preston cat hash://md5/147d1eed43249ce2ac1f8b9fb63765b1 \  
 | grep hasVersion \
 | grep "13225_2020_466_MOESM4_ESM.xlsx" \
 | preston xlsx-stream \
 | grep 'line:xlsx:hash://md5/9168998921adc01b1cf63d9cdca8342e!/data!/L' \ 
 | mlr --ijsonl --ocsv cat \
 > fungal-traits-genera.csv
```

respectively.

with first record being


```
http://www.w3.org/ns/prov#wasDerivedFrom   line:xlsx:hash://md5/9168998921adc01b1cf63d9cdca8342e!/data!/L2
http://purl.org/dc/elements/1.1/format     application/vnd.openxmlformats-officedocument.spreadsheetml.sheet
jrk_template                               jrk11009
Phylum                                     Ascomycota
Class                                      Dothideomycetes
Order                                      Asterinales
Family                                     Asterinaceae
GENUS                                      Pycnocarpon
COMMENT on genus                           
primary_lifestyle                          epiphyte
Secondary_lifestyle                        litter_saprotroph
Comment_on_lifestyle_template              
Endophytic_interaction_capability_template foliar_endophyte
Plant_pathogenic_capacity_template         
Decay_substrate_template                   leaf/fruit/seed
Decay_type_template                        
Aquatic_habitat_template                   non-aquatic
Animal_biotrophic_capacity_template        
Specific_hosts                             
Growth_form_template                       filamentous_mycelium
Fruitbody_type_template                    thyrothecium_(tiny_flattened_disc,_aperture_in_the_middle)
Hymenium_type_template                     closed
Ectomycorrhiza_exploration_type_template   
Ectomycorrhiza_lineage_template            
primary_photobiont                         
secondary_photobiont                       
column24                                   
```

## provenance 
## bill of materials 

```
<https://preston.guoda.bio> <http://www.w3.org/1999/02/22-rdf-syntax-ns#type> <http://www.w3.org/ns/prov#SoftwareAgent> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<https://preston.guoda.bio> <http://www.w3.org/1999/02/22-rdf-syntax-ns#type> <http://www.w3.org/ns/prov#Agent> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<https://preston.guoda.bio> <http://purl.org/dc/terms/description> "Preston is a software program that finds, archives and provides access to biodiversity datasets."@en <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> <http://www.w3.org/1999/02/22-rdf-syntax-ns#type> <http://www.w3.org/ns/prov#Activity> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> <http://purl.org/dc/terms/description> "A crawl event that discovers biodiversity archives."@en <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> <http://www.w3.org/ns/prov#startedAtTime> "2025-12-05T00:38:20.690Z"^^<http://www.w3.org/2001/XMLSchema#dateTime> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> <http://www.w3.org/ns/prov#wasStartedBy> <https://preston.guoda.bio> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<https://doi.org/10.5281/zenodo.1410543> <http://www.w3.org/ns/prov#usedBy> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<https://doi.org/10.5281/zenodo.1410543> <http://www.w3.org/1999/02/22-rdf-syntax-ns#type> <http://purl.org/dc/dcmitype/Software> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<https://doi.org/10.5281/zenodo.1410543> <http://purl.org/dc/terms/bibliographicCitation> "Jorrit Poelen, Icaro Alzuru, & Michael Elliott. 2018-2024. Preston: a biodiversity dataset tracker (Version 0.11.3-SNAPSHOT@07633f95a0dd9e7e07602298fc1ae57b15cf9549) [Software]. Zenodo. https://doi.org/10.5281/zenodo.1410543"@en <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<urn:uuid:0659a54f-b713-4f86-a917-5be166a14110> <http://www.w3.org/1999/02/22-rdf-syntax-ns#type> <http://www.w3.org/ns/prov#Entity> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<urn:uuid:0659a54f-b713-4f86-a917-5be166a14110> <http://purl.org/dc/terms/description> "A biodiversity dataset graph archive."@en <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> .
<hash://md5/72e125ee5986aa61f587daa41d463b35> <http://www.w3.org/ns/prov#wasGeneratedBy> <urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> <urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> .
<hash://md5/72e125ee5986aa61f587daa41d463b35> <http://www.w3.org/ns/prov#qualifiedGeneration> <urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> <urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> .
<urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> <http://www.w3.org/ns/prov#generatedAtTime> "2025-12-05T00:38:22.954Z"^^<http://www.w3.org/2001/XMLSchema#dateTime> <urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> .
<urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> <http://www.w3.org/1999/02/22-rdf-syntax-ns#type> <http://www.w3.org/ns/prov#Generation> <urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> .
<urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> <http://www.w3.org/ns/prov#wasInformedBy> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> <urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> .
<urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> <http://www.w3.org/ns/prov#used> <https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM5_ESM.xlsx> <urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> .
<https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM5_ESM.xlsx> <http://purl.org/pav/hasVersion> <hash://md5/72e125ee5986aa61f587daa41d463b35> <urn:uuid:2be1604b-995c-495b-bab7-1d346994bac6> .
<hash://md5/aa9901047720b3831f4bae6f9be235f3> <http://www.w3.org/ns/prov#wasGeneratedBy> <urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> <urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> .
<hash://md5/aa9901047720b3831f4bae6f9be235f3> <http://www.w3.org/ns/prov#qualifiedGeneration> <urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> <urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> .
<urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> <http://www.w3.org/ns/prov#generatedAtTime> "2025-12-05T00:38:23.623Z"^^<http://www.w3.org/2001/XMLSchema#dateTime> <urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> .
<urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> <http://www.w3.org/1999/02/22-rdf-syntax-ns#type> <http://www.w3.org/ns/prov#Generation> <urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> .
<urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> <http://www.w3.org/ns/prov#wasInformedBy> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> <urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> .
<urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> <http://www.w3.org/ns/prov#used> <https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM6_ESM.xlsx> <urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> .
<https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM6_ESM.xlsx> <http://purl.org/pav/hasVersion> <hash://md5/aa9901047720b3831f4bae6f9be235f3> <urn:uuid:815171b0-0b50-4ed5-a817-c60fe1aeace7> .
<hash://md5/9168998921adc01b1cf63d9cdca8342e> <http://www.w3.org/ns/prov#wasGeneratedBy> <urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> <urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> .
<hash://md5/9168998921adc01b1cf63d9cdca8342e> <http://www.w3.org/ns/prov#qualifiedGeneration> <urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> <urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> .
<urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> <http://www.w3.org/ns/prov#generatedAtTime> "2025-12-05T00:38:23.696Z"^^<http://www.w3.org/2001/XMLSchema#dateTime> <urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> .
<urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> <http://www.w3.org/1999/02/22-rdf-syntax-ns#type> <http://www.w3.org/ns/prov#Generation> <urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> .
<urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> <http://www.w3.org/ns/prov#wasInformedBy> <urn:uuid:19cfc894-9f3e-4a64-999a-818b9dd8a14b> <urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> .
<urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> <http://www.w3.org/ns/prov#used> <https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM4_ESM.xlsx> <urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> .
<https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM4_ESM.xlsx> <http://purl.org/pav/hasVersion> <hash://md5/9168998921adc01b1cf63d9cdca8342e> <urn:uuid:8aad533b-fc4c-43de-8c68-d0fa8bdc0773> .
```
