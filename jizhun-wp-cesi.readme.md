# jizhun-wp-cesi.avs

AVS1-P2 (JiZhun profile, profile_id 0x20) test stream for the FFmpeg CAVS
decoder FATE suite.

## Source

The complete bitstream `test.avs` of the conformance case
`21_cesi_6.0_frame` from the public 2009 standard conformance test set
(标准集92(2009)) for GB/T 20090.2-2006 (AVS1-P2).

- Original stream contributed by CESI and others within the AVS conformance
  programme.

## Properties

- 1920x1088, 30 fps, 3 frames
- slice-level weighted prediction (luma/chroma scale+shift per reference,
  per-MB weighting flags)
- 143,243 bytes

## Verification

Decodes bit-exactly to the reference decoder (RM52K) output of the
corresponding conformance case.
