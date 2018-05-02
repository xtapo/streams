# Video-dev group test streams

Repository hosting test streams used by https://github.com/video-dev/hls.js (and maybe others)

## 
 
## Index

- bbbAES/playlists/sample_aes/index.m3u8 (Big Buck Bunny with Sample-AES)

- issue666/playlists/cisq0gim60007xzvi505emlxx.m3u8 (Issue 666)

	- Byte-ranges into one large TS file

- test_001/stream.m3u8 (Arte TV)

	- Unencrypted
	- H264 2 resolutions, 4 bitrates each (8 bitrates total)
	- 48k AAC audio (no audio-only stream)
	- 10 seconds segments, 50 segments total (500 seconds duration)

- x36xhzz/x36xhzz.m3u8 (Big Buck Bunny)

	- Unencrypted
	- 5 qualities different in resolutions bitrate
	- Various H264 profiles (baseline, main, high)
	- PAL res and lower
	- HD + FullHD
	- Codec MIME-types given in master playlist
	- Highly encapsulated directory structure (one sub-dir per segment)

- dai-discontinuity-deltatre/manifest.m3u8 (Deltatre / BT DAI)

	- Single rendition/quality
	- AES-128 encrypted (new key per segment)
	- Codec discontinuity / Dynamic ad-inseration
	- Playlist type event (Event stream)
	- Switch to different PMT / PIDs in Transport Stream
	- Switch to unencrypted mode for ad inserted

- pts_shift/master.m3u8 (DK Turntable)

	- Unencrypted
	- 4 qualities with different bitrates and resolution
	- PTS shifted by 2.336s for all qualities
	- Provides backup stream
	- Target duration is 5s
