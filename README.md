# Streams

Repository hosting test streams used by https://github.com/video-dev/hls.js

## Index 

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
