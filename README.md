This fork of [ffmpeg-windows-build-helpers](https://github.com/rdp/ffmpeg-windows-build-helpers) serves single need: to compile FFmpeg libraries, compatible with Windows XP, that can be used by LAV Filters.

The difference with regular ffmpeg-windows-build-helpers build is that this one uses different FFmpeg repository (http://git.1f0.de/gitweb?p=ffmpeg.git;a=summary). Also this build has different (much smaller) set of enabled features (e.g. encoders and muxers are disabled since LAV Filters are only used for playback). This set is taken directly from LAV Filters.

The difference with FFmpeg libraries, provided by LAV Filters, is that this build is compatible with Windows XP (since 0.71 LAV Filters do not support Windows XP). Also this build uses GnuTLS as HTTPS backend (LAV Filters use Schannel which does not support modern TLS protocol versions on Windows XP).
