# jizhun-lowdelay-broadcom.avs

AVS1-P2 (JiZhun profile, profile_id 0x20) test stream for the FFmpeg CAVS
decoder FATE suite.

## Source

The complete bitstream `test.avs` of the conformance case
`19_broadcom_0_0_4.0` from the public 2009 standard conformance test set
(标准集92(2009)) for GB/T 20090.2-2006 (AVS1-P2).

- Original stream contributed by Broadcom within the AVS conformance
  programme.

## Properties

- 352x288, 30 fps, 5 frames
- low_delay stream: bbv_check_times in the picture header, mid-byte header
  ends with MPEG-style stuffing bytes, extension and user data blocks between
  pictures
- exercises slice start probing across multiple 0x80 stuffing bytes and
  stuffing zero runs
- 31,393 bytes

## Verification

Decodes bit-exactly to the reference decoder (RM52K) output of the
corresponding conformance case.
