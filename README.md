A [yt-dlp](https://github.com/yt-dlp/yt-dlp) extractor [plugin](https://github.com/yt-dlp/yt-dlp#plugins) to decrypt YouTube nsig using [Deno](https://deno.land)

---

The YouTube extractor first attempts with the native JSInterpreter before falling back to Deno

Pass `--extractor-args "youtube:bypass_native_jsi"` to use Deno by default

---

Deno is running in JIT-less V8 mode by default (more security at performance cost - see https://v8.dev/blog/jitless)

Pass `--extractor-args "youtube:deno_no_jitless"` to disable it.

---

*Pass `--extractor-args "youtube:bypass_native_jsi;deno_no_jitless"` to enable both extractor arguments*


## Installation

Requires yt-dlp `2023.01.02` or above.

You can install this package with pip:
```
python3 -m pip install -U https://github.com/bashonly/yt-dlp-YTNSigDeno/archive/master.zip
```

See [yt-dlp installing plugins](https://github.com/yt-dlp/yt-dlp#installing-plugins) for the many other ways this plugin package can be installed.
