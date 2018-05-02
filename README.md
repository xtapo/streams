# Video-dev group test streams

Repository hosting test streams used by https://github.com/video-dev/hls.js (and maybe others)
 
## Index

### 1) Big Buck Bunny

- Unencrypted
- 5 qualities different in resolutions bitrate
- Various H264 profiles (baseline, main, high)
- PAL res and lower
- HD + FullHD
- Codec MIME-types given in master playlist
- Highly encapsulated directory structure (one sub-dir per segment)

File: `x36xhzz/x36xhzz.m3u8`

CDN: https://rawgit.com/video-dev/streams/master/x36xhzz/x36xhzz.m3u8
	
### 2) Big Buck Bunny (sample-AES encrypted)

File: `bbbAES/playlists/sample_aes/index.m3u8`

CDN: https://rawgit.com/video-dev/streams/master/bbbAES/playlists/sample_aes/index.m3u8

### 3) Issue 666 

- Byte-ranges into one large TS file

File: `issue666/playlists/cisq0gim60007xzvi505emlxx.m3u8`

CDN: https://rawgit.com/video-dev/streams/master/issue666/playlists/cisq0gim60007xzvi505emlxx.m3u8

### 4) Arte TV VOD

- Unencrypted
- H264 2 resolutions, 4 bitrates each (8 bitrates total)
- 48k AAC audio (no audio-only stream)
- 10 seconds segments, 50 segments total (500 seconds duration)

File: `test_001/stream.m3u8`
CDN: https://rawgit.com/video-dev/streams/master/test_001/stream.m3u8

### 5) Deltatre/BT DAI discontinuity

File: `dai-discontinuity-deltatre/manifest.m3u8`

CDN: https://rawgit.com/video-dev/streams/master/dai-discontinuity-deltatre/manifest.m3u8

- Single rendition/quality
- AES-128 encrypted (new key per segment)
- Codec discontinuity / Dynamic ad-inseration
- Playlist type event (Event stream)
- Switch to different PMT / PIDs in Transport Stream
- Switch to unencrypted mode for ad inserted

### 6) DK Turntable PTS shift

File: `pts_shift/master.m3u8`

CDN: https://rawgit.com/video-dev/streams/master/pts_shift/master.m3u8

- Unencrypted
- 4 qualities with different bitrates and resolution
- PTS shifted by 2.336s for all qualities
- Provides backup stream
- Target duration is 5s
