## Philippines' Political Parties and Candidates Analysis Report

This analysis provides an exhaustive synthesis of the analytical steps, dataset treatment, and multidimensional trends uncovered from the historical database of **86,234 Philippine candidate records** spanning election years **2004 to 2016**.

### 1. Data Cleaning & Integrity Actions
Prior to performing the analysis, the dataset underwent strict preprocessing to ensure reporting accuracy:
* **Standardization**: All text features (`party`, `region`, `province`, `locality`, `position`) were stripped of leading/trailing whitespaces and converted to uniform uppercase format.
* **Handling Missing Data**: Missing values within the `locality` column (representing approximately **32%** of the dataset) were standardly classified as `PROVINCIAL LEVEL/NOT SPECIFIED` to prevent omission bias during spatial profiling.
* **De-duplication**: The dataset was verified to have no exact duplicate rows, confirming a clean, high-fidelity relational schema.

### 2. Structural & Distributional Insights

#### A. Positional Profile
Local governance positions form the vast majority of the electoral field, indicating a bottom-heavy representative hierarchy:
* **Councilors**: Make up **75.1%** of all candidate entries ($64,792$ records).
* **Mayoral and Vice-Mayoral Positions**: Comprise **9.1%** ($7,901$) and **9.1%** ($7,882$) respectively.
* **Provincial Board Members**: Account for **4.3%** ($3,747$).
* **Higher Executive Positions** (Governors, Vice Governors, and House of Representative Members) make up the remaining **2.3%** of the dataset.

#### B. Geographic Volume
Electoral competitiveness is concentrated in key geographic corridors:
* **High-Volume Centers**: **Region VIII (Eastern Visayas)** and **Region IV-A (Calabarzon)** lead candidate listings with **7,438** and **7,411** records respectively.
* **Low-Volume Centers**: **National Capital Region (NCR)** exhibits the lowest total count with only **1,627** records, reflecting concentrated city-level districts compared to sprawling municipal structures in rural regions.

### 3. Deep-Dive Political Dynamics & Trends

#### A. Temporal Coalition Shifts & Volatility
The trajectory of major political parties highlights a volatile, coalition-driven ecosystem closely aligned with national administrative transitions:
* **Lakas-CMD** held absolute dominance in 2004 with **7,353 candidates** but dropped sharply over the next decade, virtually vanishing from independent party lines by 2010 during structural reorganizations.
* **LKS-KAM** spiked to **7,435 candidates** in 2010, serving as a transitional vehicle, but collapsed to zero by 2013.
* **The Liberal Party (LP)** demonstrated the most robust growth curve, rising from a modest **1,400 candidates in 2004** to a commanding peak of **7,305 candidates in 2016**.

#### B. Regional Strongholds (Market Share %)
When normalizing regional numbers to party market shares, distinct regional fortress patterns emerge:
* **Liberal Party (LP)**: Reached its highest territorial dominance in **Region IV-A (34.2%)**, **Region VI (34.0%)**, and **Region VIII (33.2%)**.
* **Nationalist People's Coalition (NPC)**: Retains strong local bases in non-metropolitan areas, commanding **26.4% of Region II** and **23.5% of Region I**.
* **The Independent Phenomenon**: The **Cordillera Administrative Region (CAR)** presents an atypical political layout. Independent candidates (labeled `IND` and `INDEPENDENT`) hold a massive combined local market share of **30.4%** (14.8% and 15.6% respectively). This indicates that localized clan alignments and local dynamics frequently overshadow traditional national party machinery in this mountainous region.

#### C. Rise of Non-Partisan Candidates (2013 vs 2016)
By tracking the growth rate of independent filings (`IND`) during the later stage of the dataset:
* **Region IX (Zamboanga Peninsula)** experienced the most intense expansion of independent representation, surging by **+90 candidates** (from 30 in 2013 to 120 in 2016).
* **Region III (Central Luzon)** followed with an increase of **+55 candidates** (from 118 in 2013 to 173 in 2016).
* Conversely, traditional party frameworks consolidated their control in regions like **Region VIII** and **Region II**, where independent numbers declined by **-64 candidates** in each area, pointing to a strengthening of formal party networks.
