# Proposed changes to BIDS specification

This document captures all of the changes that the BEP001 team are proposing to the BIDS specification.

Table of contents:

* [Repetition Time](#repetition-time)

## Repetition Time

### Proposed Change

Adjust the definition of `RepetitionTime` in section [4.1.x Task (including resting state) imaging data](https://github.com/bids-standard/bids-specification/blob/master/src/04-modality-specific-files/01-magnetic-resonance-imaging-data.md#task-including-resting-state-imaging-data) and add two new fields to section [4.1.y Anatomy imaging data](https://github.com/bids-standard/bids-specification/blob/master/src/04-modality-specific-files/01-magnetic-resonance-imaging-data.md#anatomy-imaging-data).

### Justification

`RepetitionTime` is currently defined very specifically as relating to functional imaging data.
However there are structural scans that collect multiple volumes during an acquisition.
Here we adjust the definition of `RepetitionTime` in section 4.1.x and add `RepetitionTimeExcitation` and `RepetitionTimePreparation` as two additional terms for structural acquisitions that include multiple contrasts in 4.1.y.

