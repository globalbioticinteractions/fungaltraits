[![GloBI Review by Elton](../../actions/workflows/review.yml/badge.svg)](../../actions/workflows/review.yml) [![GloBI](https://api.globalbioticinteractions.org/interaction.svg?accordingTo=globi:globalbioticinteractions/fungaltraits&refutes=true&refutes=false)](https://globalbioticinteractions.org/?accordingTo=globi:globalbioticinteractions/fungaltraits)

Configuration to help Global Biotic Interactions (GloBI, https://globalbioticinteractions.org) index: 

Põlme, S., Abarenkov, K., Henrik Nilsson, R. et al. FungalTraits: a user-friendly traits database of fungi and fungus-like stramenopiles. Fungal Diversity 105, 1–16 (2020). https://doi.org/10.1007/s13225-020-00466-2

or

```bibtex
 @article{P_lme_2020, title={FungalTraits: a user-friendly traits database of fungi and fungus-like stramenopiles}, volume={105}, ISSN={1878-9129}, url={http://dx.doi.org/10.1007/s13225-020-00466-2}, DOI={10.1007/s13225-020-00466-2}, number={1}, journal={Fungal Diversity}, publisher={Springer Science and Business Media LLC}, author={Põlme, Sergei and Abarenkov, Kessy and Henrik Nilsson, R. and Lindahl, Björn D. and Clemmensen, Karina Engelbrecht and Kauserud, Havard and Nguyen, Nhu and Kjøller, Rasmus and Bates, Scott T. and Baldrian, Petr and Frøslev, Tobias Guldberg and Adojaan, Kristjan and Vizzini, Alfredo and Suija, Ave and Pfister, Donald and Baral, Hans-Otto and Järv, Helle and Madrid, Hugo and Nordén, Jenni and Liu, Jian-Kui and Pawlowska, Julia and Põldmaa, Kadri and Pärtel, Kadri and Runnel, Kadri and Hansen, Karen and Larsson, Karl-Henrik and Hyde, Kevin David and Sandoval-Denis, Marcelo and Smith, Matthew E. and Toome-Heller, Merje and Wijayawardene, Nalin N. and Menolli, Nelson and Reynolds, Nicole K. and Drenkhan, Rein and Maharachchikumbura, Sajeewa S. N. and Gibertoni, Tatiana B. and Læssøe, Thomas and Davis, William and Tokarev, Yuri and Corrales, Adriana and Soares, Adriene Mayra and Agan, Ahto and Machado, Alexandre Reis and Argüelles-Moyao, Andrés and Detheridge, Andrew and de Meiras-Ottoni, Angelina and Verbeken, Annemieke and Dutta, Arun Kumar and Cui, Bao-Kai and Pradeep, C. K. and Marín, César and Stanton, Daniel and Gohar, Daniyal and Wanasinghe, Dhanushka N. and Otsing, Eveli and Aslani, Farzad and Griffith, Gareth W. and Lumbsch, Thorsten H. and Grossart, Hans-Peter and Masigol, Hossein and Timling, Ina and Hiiesalu, Inga and Oja, Jane and Kupagme, John Y. and Geml, József and Alvarez-Manjarrez, Julieta and Ilves, Kai and Loit, Kaire and Adamson, Kalev and Nara, Kazuhide and Küngas, Kati and Rojas-Jimenez, Keilor and Bitenieks, Krišs and Irinyi, Laszlo and Nagy, László G. and Soonvald, Liina and Zhou, Li-Wei and Wagner, Lysett and Aime, M. Catherine and Öpik, Maarja and Mujica, María Isabel and Metsoja, Martin and Ryberg, Martin and Vasar, Martti and Murata, Masao and Nelsen, Matthew P. and Cleary, Michelle and Samarakoon, Milan C. and Doilom, Mingkwan and Bahram, Mohammad and Hagh-Doust, Niloufar and Dulya, Olesya and Johnston, Peter and Kohout, Petr and Chen, Qian and Tian, Qing and Nandi, Rajasree and Amiri, Rasekh and Perera, Rekhani Hansika and dos Santos Chikowski, Renata and Mendes-Alvarenga, Renato L. and Garibay-Orijel, Roberto and Gielen, Robin and Phookamsak, Rungtiwa and Jayawardena, Ruvishika S. and Rahimlou, Saleh and Karunarathna, Samantha C. and Tibpromma, Saowaluck and Brown, Shawn P. and Sepp, Siim-Kaarel and Mundra, Sunil and Luo, Zhu-Hua and Bose, Tanay and Vahter, Tanel and Netherway, Tarquin and Yang, Teng and May, Tom and Varga, Torda and Li, Wei and Coimbra, Victor Rafael Matos and de Oliveira, Virton Rodrigo Targino and de Lima, Vitor Xavier and Mikryukov, Vladimir S. and Lu, Yongzhong and Matsuda, Yosuke and Miyamoto, Yumiko and Kõljalg, Urmas and Tedersoo, Leho}, year={2020}, month=nov, pages={1–16} }
```

To help aid machine-readability of the data appendices of Põlme et al. 2020, snapshots of three data appendices were made using:

```
preston track --algo md5 \
 https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM5_ESM.xlsx \
 https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM6_ESM.xlsx \
https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM4_ESM.xlsx
```

then, the file ```https://static-content.springer.com/esm/art%3A10.1007%2Fs13225-020-00466-2/MediaObjects/13225_2020_466_MOESM5_ESM.xlsx``` with fingerprint ```hash://md5/72e125ee5986aa61f587daa41d463b35``` and referred to as ```Table S2. Traits of sequences. Supplementary material 5 (XLSX 56685 kb)``` was transformed in a gzip compressed tab-separated values file ```fungal-sequence-traits.tsv.gz``` using:

```bash
preston cat hash://md5/147d1eed43249ce2ac1f8b9fb63765b1 \
 | grep hasVersion \
 | grep hash://md5/72e125ee5986aa61f587daa41d463b35 \
 | preston xlsx-stream \
 | mlr --ijsonl --otsvlite cat \
 | gzip \
 > fungal-sequence-traits.tsv.gz
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
