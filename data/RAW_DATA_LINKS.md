# Raw Data Access Links (ENCODE Project)

The raw sequencing alignments (`.bam`) and continuous signal tracks (`.bigWig`) used in this pipeline are publicly available via the [ENCODE Project](https://www.encodeproject.org/).

If you intend to execute the full `01_data_extraction.ipynb` pipeline from scratch, download the following accession files and place them in their respective directories (`data/inputs/bigwig/` and `data/inputs/bam/`).

## Epigenetic Signal Tracks (.bigWig)
These files contain the raw functional genomics signals (e.g., chromatin accessibility, histone enrichment). Place these in the `data/inputs/bigwig/` directory.

| Clinical State | Accession ID | ENCODE Experiment Link |
| :--- | :--- | :--- |
| **Baseline (Normal 1)** | `ENCFF859SEG` | [ENCSR334FVC](https://www.encodeproject.org/experiments/ENCSR334FVC/) |
| **Unseen (Normal 2)** | `ENCFF055LUU` | [ENCSR979OTM](https://www.encodeproject.org/experiments/ENCSR979OTM/) |
| **Moderate Cognitive Impairment** | `ENCFF283XLM` | [ENCSR052ETC](https://www.encodeproject.org/experiments/ENCSR052ETC/) |
| **Cognitive Impairment** | `ENCFF268IZG` | [ENCSR881FDY](https://www.encodeproject.org/experiments/ENCSR881FDY/) |

## Alignment Controls (.bam)
These files contain the raw sequencing reads used to compute baseline coverage and mapping qualities to normalize the signal tracks. Place these in the `data/inputs/bam/` directory. 

*Note: To enable fast, memory-efficient positional querying across genomic coordinates, the raw `.bam` files must be indexed. You can generate the required `.bai` index files by running `samtools index <filename.bam>` in your terminal prior to executing the data handler.*

| Clinical State | Accession ID | ENCODE Experiment Link |
| :--- | :--- | :--- |
| **Baseline (Normal 1)** | `ENCFF834UNW` | [ENCSR634QZP](https://www.encodeproject.org/experiments/ENCSR634QZP/) |
| **Unseen (Normal 2)** | `ENCFF768ZXA` | [ENCSR874WOQ](https://www.encodeproject.org/experiments/ENCSR874WOQ/) |
| **Moderate Cognitive Impairment** | `ENCFF424CLY` | [ENCSR417AQU](https://www.encodeproject.org/experiments/ENCSR417AQU/) |
| **Cognitive Impairment** | `ENCFF451VHQ` | [ENCSR427DIF](https://www.encodeproject.org/experiments/ENCSR427DIF/) |