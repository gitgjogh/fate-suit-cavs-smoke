# guangdian-aec-field.avs

AVS1-P16 (Guangdian/Broadcasting profile, profile_id 0x48) test stream for
the FFmpeg CAVS decoder FATE suite.

## Source

The first 4 coded pictures of `test.avs` of the conformance case
`AVS1-P16/STEP1/83_PKU_0_0_6.0` from the public AVS1-P16 (Guangdian profile)
conformance test suite (the stream was cut at a GOP boundary).

- Author of the original stream: PKU (Peking University)
- Original purpose (from the case description): exercise field-coded B
  pictures with BFieldEnhanced set, covering the B_Skip / B_Direct_16x16 /
  SB_Direct_8x8 mode combinations of the enhanced field-B motion vector
  derivation.

## Properties

- 704x480, 25 fps, 4 frames
- AEC (arithmetic entropy coding) enabled
- adaptive weighting quantisation (AWQ) enabled
- field-coded pictures (picture_structure = field) with the enhanced
  field-P/field-B modes (pb_field_enhanced_flag)
- 19,327 bytes

## Verification

Decodes bit-exactly to the prefix of the reference decoder (GDM4.2) output
of the corresponding conformance case.
