# jizhun-field-cesi.avs

AVS1-P2 (JiZhun profile, profile_id 0x20) test stream for the FFmpeg CAVS
decoder FATE suite.

## Source

The complete bitstream `test.avs` of the conformance case
`01_cesi_step5_4.0_field` from the public 2009 standard conformance test set
(标准集92(2009)) for GB/T 20090.2-2006 (AVS1-P2).

- Original stream contributed by CESI and others within the AVS conformance
  programme.

## Properties

- 352x288, 25 fps, 7 frames
- field-coded pictures (picture_structure = field) in a progressive sequence
- 22,997 bytes

## Verification

Decodes bit-exactly to the reference decoder (RM52K) output of the
corresponding conformance case.
