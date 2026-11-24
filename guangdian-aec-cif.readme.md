# guangdian-aec-cif.avs

AVS1-P16 (Guangdian/Broadcasting profile, profile_id 0x48) test stream for
the FFmpeg CAVS decoder FATE suite.

## Source

The complete bitstream `test.avs` of the conformance case
`AVS1-P16/STEP1/35_Tsinghua_HS_0_0_0x48` from the public AVS1-P16 (Guangdian
profile) conformance test suite.

- Author of the original stream: Tsinghua University
- Original purpose (from the case readme): test the range coverage of the AEC
  (arithmetic entropy coding) syntax elements mb_skip_run, mb_qp_delta,
  mb_reference_index (P pictures) and mb_type.

## Properties

- 352x288, 25 fps, 4 frames (4 coded pictures)
- AEC (arithmetic entropy coding) enabled
- interlaced sequence with progressive (frame) pictures
- 187,845 bytes

## Verification

Decodes bit-exactly to the reference decoder (GDM4.2) output of the
corresponding conformance case.
