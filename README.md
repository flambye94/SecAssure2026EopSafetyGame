# SecAssure2026EopSafetyGame

Supplementary research material and prototype interface documentation for the paper:

> **A Safety-Aware Elevation of Privilege Game for ICS Threat Modeling Education: Experience from Three Workshop Iterations on Smart Grid Purdue Models**
> Fabien Sechi and Nadia Saad Noori

This repository supports ongoing research on a safety-aware adaptation of Adam Shostack’s **Elevation of Privilege (EoP)** threat-modeling card game for **Industrial Control Systems (ICS)** and **Smart Grid cybersecurity education**.

The project adapts EoP to an IT/OT context by anchoring threat modeling in a **Smart Grid Purdue-model architecture** and by adding an explicit **Safety/HSE impact dimension** to every identified threat. The purpose is to help participants reason not only about cyber impact, but also about possible physical and operational consequences such as equipment damage, grid instability, loss of operator visibility, or risk to field personnel.

## Repository purpose

This repository is intended to make the research artefacts available for review, replication, teaching, and future development.

It currently includes:

* the research paper or paper-related supplementary material;
* an anonymised Excel workbook containing research interview and workshop data;
* facilitator coding tables and consolidated threat-modeling outputs;
* Safety/HSE impact assessments and cyber-severity ratings;
* screenshots of the current application prototype;
* material supporting future development of a runnable Safety-Aware EoP demonstrator.

The repository is therefore both a **research archive** and a **development support space** for the next version of the safety-aware threat-modeling game.

## Current status

The project is a work in progress.

At this stage, the PDF interface document does **not** represent a complete user manual or a validated software release. It contains screenshots of the application prototype developed to support future research and development.

The Excel file contains anonymised research material and should be treated as supplementary research data. It is included to support transparency and reproducibility while protecting participant identity.

## Research context

The work builds on three workshop iterations of a Safety-Aware Elevation of Privilege game:

1. a Norwegian cybersecurity conference workshop;
2. a university Capture-the-Flag student session;
3. a university master-student session using explicit Safety/HSE tagging.

Across these iterations, the research explored how participants identify threats in a Smart Grid ICS architecture, how they use STRIDE categories, and how they reason about the safety consequences of cyber threats.

The central research observation is that **safety reasoning does not reliably emerge on its own in threat-modeling exercises**. It must be structurally prompted by the game design. For this reason, the Safety/HSE impact field is treated as a core part of the modified game.

## Game concept

The original Elevation of Privilege game uses the STRIDE taxonomy:

* Spoofing
* Tampering
* Repudiation
* Information disclosure
* Denial of service
* Elevation of privilege

This project keeps the accessible, card-based, discussion-oriented nature of EoP, but modifies it for ICS and Smart Grid education through five design changes.

| ID | Modification                         | Purpose                                                             |
| -- | ------------------------------------ | ------------------------------------------------------------------- |
| M1 | Smart Grid Purdue-model architecture | Anchors every threat in a concrete IT/OT system                     |
| M2 | Explicit attacker goal               | Connects technical threats to operational and societal consequences |
| M3 | Safety/HSE impact dimension          | Makes physical safety a first-class part of threat modeling         |
| M4 | Structured threat template           | Records threats in a comparable and auditable format                |
| M5 | One-card-per-category rotation       | Encourages broader STRIDE coverage                                  |

## Safety/HSE impact dimension

Each accepted threat is assigned a Safety/HSE impact level.

| Level      | Meaning                                                                                                           |
| ---------- | ----------------------------------------------------------------------------------------------------------------- |
| High       | Plausible direct risk of injury, major outage, severe equipment damage, environmental impact, or grid instability |
| Medium     | Contributes to unsafe conditions, delayed response, loss of visibility, or weakening of a protection layer        |
| Low / None | Mainly financial, reputational, or confidentiality-related impact with no clear path to physical harm             |

This rating is not intended to replace a formal safety analysis. It is a pedagogical and research prompt designed to make participants discuss the physical consequences of cyber threats in ICS environments.

## Application prototype

The repository also documents the current application prototype developed to support future versions of the game.

The interface showcase PDF currently includes screenshots of the following prototype views:

* backend connection screen;
* home screen with separate paths for players and facilitators;
* guided game board;
* projected room and join screen;
* structured threat register;
* debrief dashboard;
* cyber, safety, and cyber-safety risk matrices;
* editable Smart Grid Purdue-model target architecture.

The prototype is designed around a local-first setup. The current version supports a local realtime backend, while hosted online play is marked as future work.

The application aims to support facilitators by making the workshop structure visible during play:

* the attacker goal remains visible;
* the Smart Grid Purdue architecture is available during threat identification;
* the STRIDE rotation is shown;
* every threat must be entered using a structured template;
* the Safety/HSE impact tag is mandatory;
* accepted threats can be reviewed in a register;
* debrief dashboards support cross-group discussion.

## Data and supplementary material

The anonymised Excel workbook contains research material from the workshop iterations and interviews. Depending on the sheet, it may include:

* anonymised participant or group identifiers;
* threat names and descriptions;
* STRIDE categories;
* affected devices, links, or Purdue layers;
* cyber-severity ratings;
* Safety/HSE impact ratings;
* facilitator notes;
* coding decisions;
* consolidated observations.

This material is provided for research transparency, replication, and future evaluation. It should not be interpreted as a statistically validated dataset. The workshop results are exploratory and should be read in the context of an experience report.

## Suggested use

This repository may be useful for:

* cybersecurity education;
* ICS and OT security courses;
* Smart Grid threat-modeling exercises;
* safety-security co-engineering workshops;
* game-based learning research;
* replication of the Safety-Aware EoP workshop;
* development of future digital threat-modeling tools.

The game is best used as an early-stage learning and discussion activity before deeper technical analysis, formal safety assessment, or mitigation design.

## Suggested workflow for researchers and instructors

1. Read the paper to understand the research motivation and workshop protocol.
2. Review the anonymised Excel file to inspect the workshop outputs.
3. Use the interface-showcase PDF to understand the current prototype direction.
4. Adapt the Smart Grid Purdue architecture or threat template to your own teaching context.
5. Run the game with participants.
6. Compare the resulting threats, STRIDE coverage, and Safety/HSE reasoning with the existing anonymised dataset.

## Limitations

The material in this repository should be interpreted with the following limitations in mind:

* the workshop data is anonymised and exploratory;
* the number of participants is limited;
* the protocol evolved across workshop iterations;
* the Safety/HSE ratings are pedagogical prompts, not formal safety assessments;
* the application screenshots show a prototype interface, not a finished software product;
* the current PDF is intended to support future development and communication, not to serve as full technical documentation.

## Future work

Future development may include:

* a complete facilitator guide;
* a runnable and documented version of the application;
* improved support for online play;
* export functions for research data;
* refined cyber-safety scoring;
* additional ICS scenarios beyond Smart Grid;
* integration with formal safety-security taxonomies;
* pre- and post-workshop evaluation instruments;
* larger validation studies with students and practitioners.

## Citation

If you use this repository, please cite the accompanying paper:

```bibtex
@inproceedings{sechi2026safetyawareeop,
  title     = {A Safety-Aware Elevation of Privilege Game for ICS Threat Modeling Education: Experience from Three Workshop Iterations on Smart Grid Purdue Models},
  author    = {Sechi, Fabien and Saad Noori, Nadia},
  year      = {2026}
}
```

## Contact

For questions about the paper, anonymised dataset, workshop protocol, or application prototype, please contact the authors through this repository.
