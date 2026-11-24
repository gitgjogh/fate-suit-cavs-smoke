# jizhun-422-hisilicon.avs

AVS1-P2 (JiZhun profile, profile_id 0x20) test stream for the FFmpeg CAVS
decoder FATE suite.

## Source

The first 4 coded pictures of `test.avs` of the conformance case
`AVS1-P2_JZP09/FINAL/30_Hisilicon_0_0_0x42` from the public AVS1-P2 (JiZhun
profile) JZP09 conformance test suite (the stream was cut at a GOP boundary).

- Author of the original stream: HiSilicon
- Original purpose (from the case description): 4:2:2 chroma format decoding;
  the syntax element cbp_422 covers all its possible values.

## Properties

- 720x576, 30 fps, 4 frames, 4:2:2 chroma (YUV422P output)
- CBP422 (second coded block pattern for the lower chroma 8x8 blocks)
- 154,007 bytes

## Verification

Decodes bit-exactly to the prefix of the reference decoder (RM52K) output of
the corresponding conformance case.
