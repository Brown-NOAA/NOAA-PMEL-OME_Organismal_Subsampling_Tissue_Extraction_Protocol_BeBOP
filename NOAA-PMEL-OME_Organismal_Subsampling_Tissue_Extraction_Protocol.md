---
# MIOP terms
methodology_category: sample collection, sample extraction
project: NOAA Pacific Marine Environmental Laboratory Ocean Molecular Ecology Group protocols
purpose: biodiversity assessment objective [OBI:0001969]
analyses: individual organism specimen [OBI:0002648], sample from organism [OBI:0000671], DNA extraction [OBI:0000257]
geographic_location: North East Pacific Ocean [GAZ:00013765], Bering Sea [GAZ:00008990], Arctic Ocean [GAZ:00000323], South Pacific Ocean [GAZ:00002418]
broad_scale_environmental_context: marine biome [ENVO:00000447], marine photic zone [ENVO:00000209]
local_environmental_context: oceanic epipelagic zone biome [ENVO:01000035], marine benthic biome [ENVO:01000024], estuary [ENVO:00000045]
environmental_medium: HAN HELP
target: deoxyribonucleic acid (DNA) [NCIT:C449]
creator: Han Weinrich, Karina Lai
materials_required: vortexer [OBI:0400118], centrifuge [OBI:0400106], incubator [OBI:0000136]
skills_required: sterile technique, pipetting skills, standard molecular technique
time_required: 420
personnel_required: 1
language: en
issued: 2025-10-10
audience: scientists
publisher: NOAA Pacific Marine Environmental Laboratory Ocean Molecular Ecology Program; University of Washington Cooperative Institute for Climate, Ocean, & Ecosystem Studies
hasVersion: 1
license: CC0 1.0 Universal
maturity level: mature

# FAIRe terms
samp_category: sample
env_broad_scale: marine biome [ENVO:00000447], marine photic zone [ENVO:00000209], freshwater biome [ENVO:00000873]
env_local_scale: oceanic epipelagic zone biome [ENVO:01000035], marine benthic biome [ENVO:01000024], estuary [ENVO:00000045]
env_medium: HAN HELP
habitat_natural_artificial_0_1: 0
samp_collect_method: ROV grab, hand-sampling
samp_collect_device: ROV, bucket
samp_size: not applicable
samp_size_unit: not applicable
samp_vol_we_dna_ext: not applicable
samp_vol_we_dna_ext_unit: not applicable
nucl_acid_ext_lysis: physical | enzymatic | thermal
nucl_acid_ext_sep: column-based
nucl_acid_ext: 
nucl_acid_ext_kit: Qiagen DNeasy Blood and Tissue Kit, 250
nucl_acid_ext_modify: Modified for small, calcareous organisms, reagent volume altered
dna_cleanup_0_1: 0
dna_cleanup_method: not applicable
concentration: not applicable
concentration_method: not applicable
ratioOfAbsorbance260_280: not applicable
pool_dna_num: not applicable
nucl_acid_ext_method_additional: not applicable
---

# NOAA PMEL OME Protocol for Organismal Subsampling and Tissue Extraction

## PROTOCOL INFORMATION

### Minimum Information about an Omics Protocol (MIOP)

- MIOP terms are listed in the YAML frontmatter of this page.
- See <https://github.com/BeBOP-OBON/miop/blob/main/model/schema/terms.yaml> for list and definitions.

### Making eDNA FAIR (FAIRe)

- FAIRe terms are listed in the YAML frontmatter of this page.
- See <https://fair-edna.github.io/download.html> for the FAIRe checklist and more information.
- See <https://fair-edna.github.io/guidelines.html#missing-values> for guidelines on missing values that can be used for missing FAIRe or MIOP terms.

### Authors

- All authors known to have contributed to the preparation of this protocol, including those who filled in the template.
- Visit https://orcid.org/ to register for an ORCID.
- Date is the date the author first worked on the protocol.

| PREPARED BY All authors known to have contributed to the preparation of this protocol, including those who filled in the template.  | AFFILIATION | ORCID (visit https://orcid.org/ to register) | DATE |
| ------------- | ------------- | ------------- | ------------- |
| Shannon Brown | Ocean Molecular Ecology, NOAA PMEL & UW CICOES  | 0000-0001-9808-2638 |2025-10-06|
| Karina Lai  | Ocean Molecular Ecology, NOAA PMEL & UW CICOES  | 0009-0008-9236-6128 |2025-10-06|

### Related Protocols

- This section contains protocols that should be known to users of this protocol.
- Include the link to each protocol.
- Include the version number and release date (if available).
- Internal/External: "Internal" are derivative or altered protocols, or other protocols in this workflow. "External" are protocols from manufacturers or other groups.

| PROTOCOL NAME | LINK         | VERSION      | RELEASE DATE | INTERNAL/EXTERNAL |
| ------------- | ------------ | ------------ | ------------ | ----------------- |
| NOAA-PMEL-OME_Qubit_Quantification_Protocol_BeBOP | [https://github.com/HanWeinrich/NOAA-PMEL-OME-Qubit-Quantification-Protocol-BeBOP/blob/main/NOAA-PMEL-OME-Qubit-Quantification-Protocol-BeBOP.md](https://github.com/HanWeinrich/NOAA-PMEL-OME-Qubit-Quantification-Protocol-BeBOP/blob/main/NOAA-PMEL-OME_Qubit_Quantification_Protocol_BeBOP.md) | 1.0.1  |2025-08-22| Internal |
| Introduction to Developing DNA Reference Barcode Sequences |[https://doi.org/10.5281/zenodo.14867762](https://doi.org/10.5281/zenodo.14867762) | 1.0.0  | 2025-02-19  | External |

### Protocol Revision Record

- Version numbers start at 1.0.0 when the protocol is first completed and will increase when changes that impact the outcome of the procedure are made (patches: 1.0.1; minor changes: 1.1.0; major changes: 2.0.0).
- Release date is the date when a given protocol version was finalised.
- Description of revisions includes a brief description of what was changed relative to the previous version.

| VERSION | RELEASE DATE | DESCRIPTION OF REVISIONS |
| ------------- | ------------- | ------------- |
| 1.0.0 | 2025-10-10 | Initial release |

| ACRONYM / ABBREVIATION | DEFINITION |
| ------------- | ------------- |
|CICOES| Cooperative Institute for Climate, Ocean, and Ecosystem Studies|
|DNA	|Deoxyribonucleic acid|
|EtOH| Ethanol|
|NOAA|National Oceanic and Atmospheric Administration|
|OME	|Ocean Molecular Ecology|
|PME|Pacific Marine Environmental Laboratory
|PPE | Personal protective equipment |
|UV| Ultraviolet|
|UW| University of Washington|

### Glossary

| SPECIALISED TERM | DEFINITION |
| ------------- | ------------- |
| No template control | PCR negative control. Typically, nuclease-free water is loaded in place of a sample on a PCR to control for contamination in the PCR step. |

## BACKGROUND

This document outlines the standard protocol for subsampling and extracting DNA from organismal tissue. 

### Summary

The NOAA PMEL Ocean Molecular Ecology (OME) follows guidance set by the [Introduction to Developing DNA Reference Barcode Sequences](https://doi.org/10.5281/zenodo.14867762) to collect and subsample organisms. Nucleic acid extraction using the Qiagen DNeasy Blood and Tissue Kit, with some modifications to the manufacturer’s protocol, is also used by this group to extract DNA from organismal tissue.

### Method Description and Rationale

The [Introduction to Developing DNA Reference Barcode Sequences](https://doi.org/10.5281/zenodo.14867762) works to establish a highly reproducible and easily executable sampling protocol for organisms. DNeasy Blood & Tissue kits are commonly used for tissue extractions across many phyla.

### Spatial Coverage and Environment(s) of Relevance

This protocol has been used to subsample tissue and extract DNA from hundreds of organismal samples taken from coastal stations off the western coast of North America in the Northeastern Pacific Ocean, Bering Sea, and Arctic Ocean (primarily off California, Oregon, Washington, and Alaska). Samples collected range in depth from surface ocean (epipelagic biome) to just off bottom (benthic biome) at varying distances from shore (coastal to off-shelf).

### Personnel Required

One person with molecular biology experience.

### Safety

Buffer AW1 from the DNeasy Blood & Tissue Kit contains guanidine hydrochloride and is classified as category 4 for acute toxicity [(Safety Data Sheet)](https://www.qiagen.com/binary/resource/sds/800000000214-en-GB-IE--1/214-BufferAW1-en-GB-IE--1.00000.pdf). Additional care should be taken when working with this buffer. Highly reactive compounds can form if Buffer AL or AW1 is combined with bleach. For other reagents, standard precautions, including wearing PPE, should be taken to avoid skin and eye exposure to chemicals.

### Training Requirements

Molecular biology training (including, at a minimum, sterile technique, pipetting small volumes, and previous DNA/RNA extraction experience) is required to conduct this protocol.

### Time Required to Execute the Procedure

Subsampling and extraction from a sample can vary depending on the size and type of tissue. Incubation during lysis is normally completed in 1-3 hours, depending on the tissue. After lysis, the DNeasy Blood & Tissue spin-column procedure can be completed in 20 minutes.

## EQUIPMENT

- Description: E.g., "filter".
- Product Name and Model: Provide the official name of the product.
- Manufacturer: Provide the name of the manufacturer of the product.
- Quantity: Provide quantities necessary for one application of the standard operating procedure (e.g., number of filters).
- Remark: For example, some of the consumables may need to be sterilized, some commercial solutions may need to be diluted or shielded from light during the operating procedure.

For a full extraction set, including 24 organismal samples:

| DESCRIPTION | PRODUCT NAME AND MODEL | MANUFACTURER | QUANTITY | REMARK |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| **Durable equipment** |||||||
| Heatshaker | Fisherbrand incubating mini-shaker | Fisher Scientific | 1 | Can be substituted with generic; hot bath not recommend for sterility reasons. |
| Centrifuge | Eppendorf 5425 R  | Fisher Scientific | 1 | Can be substituted with generic, but needs to fit 1.5 mL tubes. |
| Vortex | Analog vortex mixer | Fisher Scientific | 1 | Can be substituted with generic. |
| UV crosslinker | UV crosslinker AH (115V), 234100 | Boekel Scientific  | 1 | Recommended not required, but can be substituted. |
|-20°C freezer|TSX high-performance -20°C manual defrost freezer |Fisher Scientific|1|Can be substituted with a generic, but recommend temperature display.|
|Pipettor: 20 - 200 μL	|Pipetman P200L|Gilson|	1|Can be substituted with any accurate pipettor.|
|Pipettor: 100-1000 μL	|Pipetman P1000	|Gilson	|1|Can be substituted with any accurate pipettor.|
| Microtube racks | 96-Well flipper microtube racks | Fisher Scientific | 2 | Can be substituted with generic, but must fit 1.5-2.0 mL tubes. |
| 50 mL tube racks | SPL snap 50 mL tube rack (25 place) | SPL Life Sciences | 2 | Can be substituted, but must fit sterivex. |
| 4-way tube racks | 4 way interlocking tube rack| Cole-Parmer | 4 | Can be substituted with generic, but must fit 12 x 5 mL tubes and 50 mL tubes. |
|Wash bottles|Safety wash bottles 500 mL for EtOH and bleach|VWR|2|Can be substituted with generic, but recommend different colored bottles for each reagent. Must be sterilized before use. |
| **Consumable equipment** |
| 200 μL pipette tips  | TipOne RPT filter tips 200 μL graduated| USA Scientific |96 | Can be substitued with generic. Must be sterile and filtered. |
| 1000 μL pipette tips  | TipOne RPT filter tips 1000 μL | USA Scientific |220 | Can be substituted with generic. Must be sterile and filtered. |
| 1.5 mL tubes | Snap cap DNA LoBind 1.5 mL tubes, PCR-clean| Eppendorf |24 | Can be substituted with generic. Must be sterile. |
| 5 mL tubes | DNA LoBind 5 mL PCR clean centrifuge tube | Eppendorf | 24 | Can be substituted with generic. Must be sterile/PCR clean. |
| 50 mL falcon tubes | Falcon 50 mL high clarity conical centrifuge tube | Corning Falcon | 3 | Can be substituted with generic. Must be sterile. |
| Kimwipes | Delicate task wipes | Kimtech | 5 | Can be substituted with generic. Must be lint-free.|
| Nitrile gloves | Powder free nitrile gloves | Fisher Scientific | 8 | Can be substituted with generic nitrile gloves. Does not come sterile; it must be sterilized before use.|
| Lab notebook | Durable, hardcover lab notebook | Generic | 1 | Dedicated to the lab space.|
| Rite in the Rain paper | All weather paper | Rite In The Rain | 1 ||
| Writing utensils | Sharpies and pens | Generic | 2 | Dedicated to the lab extraction space. Not made of wood - must be able to be wiped down with bleach/EtOH.  |
| **QIAGEN Extraction Kit** | Qiagen DNeasy Blood and Tissue Kit - 250 extractions | QIAGEN | 1 | For this protocol at scale (i.e., 250 samples), additional volumes of some buffers need to be purchased.|
| *QIAGEN kit consumables* |  |  |  |  |
| Spin columns | Mini spin column | **Included in kit** | 24 | Kit contains 250 columns - sufficient for 250 extractions using this protocol. |
| Collection tubes | 2 mL collection tube | **Included in kit**| 48 | Kit contains 500 tubes - sufficient for 250 extractions using this protocol. |
| *QIAGEN kit chemicals* |  |  |  |  |
| Buffer ATL | QIAGEN Buffer ATL | **Included in kit** | 4.5 mL | Kit contains 50 mL  - sufficient for 250 extractions. |
| Proteinase K | Qiagen Proteinase K | **Included in kit** | 500  μL  | Kit contains 6 mL - sufficient for 250 extractions. |
| Buffer AL | Qiagen Buffer AL | **Included in kit** | 5.0 mL | Kit contains 66 mL - sufficient for 250 extractions. |
| Buffer AW1 | Qiagen Buffer AW1 | **Included in kit** | 12 mL | Kit contains 98 mL concentrate - sufficient for 250 extractions. **Mix with 100% molecular grade EtOH before use, instructions on bottle** |
| Buffer AW2 | Qiagen Buffer AW2| **Included in kit** | 12 mL| Kit contains 66 mL concentrate - sufficient for 250 extractions using this protocol. **Mix with 100% molecular grade EtOH before use, instructions on bottle** |
| Buffer AE | Qiagen Buffer AE | **Included in kit** | 2400 μL | Kit contains 120 mL - sufficient for 1200 extractions. |
| **Chemicals** |
| 100% molecular grade EtOH | 200 proof molecular biology grade ethanol | Fisher Scientific | 30 mL|Can be substituted with generic, must be 200 proof and molecular biology grade. |
| 70% EtOH | Molecular biology grade ethanol | 20 mL |  |
| 10% bleach | Hypochlorite bleach | Clorox | 10 mL| Remake every ~5 days as bleach decomposes quickly at 10% concentration. The majority is used in bottle/tube sterilization.|

## STANDARD OPERATING PROCEDURE

### Field Collection and Subsampling
For more details on organismal collection, see [Introduction to Developing DNA Reference Barcode Sequences](https://doi.org/10.5281/zenodo.14867762).

Organisms can be collected via a variety of methods (e.g., hand-sampling, scuba survey, ROV sampling). Collect live, intact specimens to ensure quality for sorting, processing, photography, and DNA barcoding. Maintain the temperature, oxygen, and water levels, as DNA degrades after cell death. Some species (e.g., gelatinous invertebrates, shrimp) require fresh specimens for identification, while others (e.g., fishes) can be preserved. Live color and delicate features often degrade under stress, so photographing live specimens is essential.

**General Photography Guidelines**
* Photograph all organisms with a scale bar and their sampling number before subsampling.
*  For the best quality photo, fully submerge the specimen in seawater, place black felt under the bin, and elevate using Falcon tube caps. Then use a DSLR and flash.
*  In addition to a standard photo of the entire organism, prioritize anterior and posterior photos for polychaetes and oral and aboral photos of other organisms (e.g., clams, stars, anemones). If the organism has unique features or appendages, capture photos as well.
Additional photo suggestions can be found below by taxon.

#### Tissue Subsampling
Ideal genetic subsamples are a couple of cubic millimeters, in ~1 mm sized pieces, and are taken when organisms are sampled in the field. Once the organism is subsampled, place the tissue in a 1.5 mL tube and ensure you use ~10x the volume of fixative. With small animals or those that deteriorate rapidly (sponges, flatworms, etc.), it is important to fix a subsample before or quickly after death, as DNA degrades rapidly. If the time or setting doesn't allow for field subsampling, this process can occur back in the laboratory for less sensitive specimens.

1.  Sterilize benches and durable equipment by wiping with 10% bleach followed by 70% EtOH. For extra caution, sterilize forceps used for subsampling by dipping in 70% EtOH and flame sterilizing. 
2.  Place the sample on a flat surface or dissection tray, then use sterilized equipment to subsample the organism - see guidance below for each taxon.
3.  Place specimen in pre-labeled 1.5 mL collection tube pre-filled with 96% EtOH. Place the sampling number (printed on Rite in the Rain paper) in the collection tube alongside the specimen.
4.  Wipe down the dissection tray with paper towels between samples and resterilize equipment.

#### Procedures by Taxon
* **Porifera:** Specimen photos are important for identification (e.g., color, texture, associated species). DNA subsample from exterior wall tissue.
* **Soft corals, gorgonians, and black corals:** Subsample exterior walls or soft appendages.
* **Anemones:** Subsample tentacle. Photos of live animals needed for speciation (i.e., coloration).
* **Stony corals and hydrocorals:** Small colony fragments from a tissue scrape work for a subsample.
* **Flatworms:** Specimen photos are necessary for ID; take snippet of exterior end for genetic work
* **Worms:** Easier to photograph if relaxed via refrigeration; take a snippet of abdominal, posterior, or anterior muscular tissue for a genetic subsample.
* **Crustaceans:** When photographing crabs, it’s best to photograph freshly killed animals with legs spread. However, for shrimp and other translucent species, living photos are better. Kill decapods by freezing them. A tissue sample extracted from a leg, pleopod in shrimp, or abdomen and fixed in concentrated ethanol provides a good additional genetic sample.
* **Mollusks:** Photos are most useful for opisthobranchs and cephalopods, but also for the soft body of any species. A good technique for shelled mollusks where shell and tissue are desired is to microwave them for 0.5-2 minutes in a high-power microwave; this blows the animal out of its shell, and then the body fixes well and is accessible without breaking the shell. Microwaving does not destroy the DNA.
* **Asteroids and ophiuroids:** Relax specimens via refrigeration. Associated field photos and genetic ethanol subsamples are important. For large stars, this can be snipped tube feet, or hepatic caeca/gonad extracted from the body prior to fixation. 
* **Crinoids:** Subsample exterior appendage; sample and photograph associated commensals.
* **Holothuroids:** A subsample of tentacle, tube feet, or internal organs useful for DNA.  
* **Echinoids:** Can relax in the fridge. A subsample of tube feet, or gonad/gut, taken with forceps inserted through a cut in the peristomal membrane provides a useful tissue sample.  
* **Ascidians:** Take a snippet of the inner part of siphons in ethanol of larger solitary species or of chopped up bits of colony for DNA. Best to fix a good piece of colonial species for DNA, so zooids can be pulled for extraction later, so use a larger vial for that. Photos are very useful.

### Storage - Organismal Samples
Full organismal samples stored in 70% EtOH can be stored in a dry storage room at room temperature. Tissue samples should be stored in a -20°C freezer until extracted.

### Preparation - Tissue Extraction

Protocol can be carried out in a general laboratory space, separated from areas designated for low-biomass bench work. 

1. Sterilize benches and durable equipment by wiping with 10% bleach followed by 70% EtOH. 
2. For extra caution, sterilize forceps used for subsampling by dipping in 70% EtOH and flame sterilizing. 
3. Turn on the heatshaker to 56°C. If the Buffer ATL or AL has precipitate, place it in a heatshaker. Allow the buffer to heat until all precipitate is gone (~15 minutes), swirl as needed.
4. Aliquot ~25 mL of 100% EtOH into a 50 mL Falcon tube and store at -20°C freezer for later use.
5. Ensure 100% molecular grade EtOH has been added to Buffer AW1 and AW2 according to the Qiagen DNeasy Blood and Tissue Kit manufacturer's instructions. 

#### Subsample Preparation
If the subsample is too large (> ~1 mm), use a sterilized razor blade and forceps to break off a small piece and relocate it to a new 1.5 mL tube. Cutting the tissue into smaller pieces has been found to result in more efficient lysis. If you are dealing with a hard-shelled organism (e.g., gastropod), use a sterilized mortar and pestle to break down the hard outer shell and access the soft tissue for extraction. 

### Tissue Extraction
For most organismal samples, the standard QIAGEN Blood & Tissue protocol (Option A) as follows works for extracting DNA. However, for some smaller specimens (e.g., larval stage organisms, eggs) and/or organisms with a calcarious outer shell (e.g., pteropods, orphurioids), a modified protocol (Option B) with smaller volumes is more effective.

1. In the 1.5 mL tube with the subsampled tissue, add 180 μL Buffer ATL (Option A) or 45 μL (Option B).
2. Add 20 μL Proteinase K (Option A) or 5 μL (Option B) and mix by vortexing. 
3. Incubate in a heatshaker at 56°C until the tissue is completely lysed. Lysis time varies depending on the type of tissue, but is typically completed in 1-3 hours.

**Note**: Lysate may appear viscous but should not be gelatinous as it may clog the DNeasy Mini spin column. 

4. Vortex for 15 seconds. Add 200 μL Buffer AL (Option A) or 50 μL (Option B) and vortex again. 
5. Add 200 μL cold EtOH (Option A) or 50 μL (Option B) and vortex.

**Note**: A white precipitate may form on the addition of Buffer AL and EtOH. This will not disrupt the DNeasy procedure. 

6. Pipette the mixture 600 μL (Option A) or 150 μL (Option B) into the DNeasy Mini spin column placed in a 2 mL collection tube. 
7. Centrifuge at ≥6000 x g (8,000 rpm) for 1 min. Discard the flow-through and collection tube. 
9. Place the DNeasy Mini spin column into a new 2 mL collection tube and add 500 μL Buffer AW1.
9. Centrifuge at ≥6000 x g (8,000 rpm) for 1 min. Discard the flow-through and collection tube. 
10. Place the DNeasy Mini spin column into a new 2 mL collection tube and add 500 μL Buffer AW2.
11. Centrifuge for 3 min at 20,000 x g (14,000 rpm). 
12. Discard flow-through and collection tube. 
13. Place the DNeasy Mini spin column in a sterile, labeled 1.5 mL tube. 
14. Pipette 100 µL Buffer AE onto the spin column membrane. Incubate for 5 min and then centrifuge for 1 min at 6,000 ∗ g (8,000 rpm). Without discarding flow-through, repeat with another 100 µl Buffer AE and centrifuge. Discard the spin column, as your extract is now in the 1.5 mL tube.
15. Store extracted DNA tubes in a -20℃ freezer until later use.

### Storage - Tissue Extractions

Place extracted DNA tubes into a labeled cryobox and store in a -20°C freezer until later use. Preferably, set aside an aliquot for long-term storage to be archived in a -80°C freezer.

### Quality Control

Samples and controls are quantified to verify DNA concentration using the [NOAA-PMEL-OME-Qubit-Quantification-Protocol-BeBOP](https://github.com/HanWeinrich/NOAA-PMEL-OME-Qubit-Quantification-Protocol-BeBOP/blob/main/NOAA-PMEL-OME_Qubit_Quantification_Protocol.md). Lastly, samples are PCR amplified alongside no template and positive controls.

### Basic Troubleshooting Guide

**Issue 1:** Column clogging when pipetting the sample/Buffer AL/EtOH mixture to the spin columns

**Solution:** If a sample is turbid, solids may survive the digestion and lysis steps. These solids can clog the spin column and trap liquid above the filter. If repeating the spin-down step does not fully drain liquid from the column, use a second fresh column for the remainder of the sample. Both spin columns are then run through the protocol, and the eluted DNA is combined.

**Issue 2:** Liquid on sides of collection tube after centrifuge step following Buffer AW2 addition.

**Solution 2:** Re-run the spin-down step in a fresh spin column. No additional buffer AW2 is added. If the issue persists, move to a new collection tube and respin.

**Record troubleshooting notes and issues in the lab notebook.**

## REFERENCES

The West Coast Ocean Biomolecular Observing Network, Gold, Z., Brown, S., Collins, A., Girard, M., Goodwin, K., McAllister, S., Meyer, C., Parsons, K., Patin, N., Rouse, G., Sala, L., Satterthwaite, E., Seid, C., Theroux, S., and Wetzer, R. (2025): Introduction to Developing DNA Reference Barcode Sequences (v1.0). Zenodo. [https://doi.org/10.5281/zenodo.14867763](https://doi.org/10.5281/zenodo.14867763)
