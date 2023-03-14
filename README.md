A [yt-dlp](https://github.com/yt-dlp/yt-dlp) extractor [plugin](https://github.com/yt-dlp/yt-dlp#plugins) to decrypt YouTube nsig using [Deno](https://deno.land)

---

The YouTube extractor first attempts with the native JSInterpreter before falling back to Deno

Pass `--extractor-args "youtube:bypass_native_jsi"` to use Deno by default

---

Deno is running in JIT-less V8 mode by default (more security at performance cost - see https://v8.dev/blog/jitless, also [this](https://gist.github.com/sakura4919/df97467b169579e00f30d9049b15ab67?permalink_comment_id=4297519#gistcomment-4297519))  

Pass `--extractor-args "youtube:deno_no_jitless"` to disable it.

*(pass `--extractor-args "youtube:bypass_native_jsi;deno_no_jitless"` to enable both extractor arguments)*


## Installation

Requires yt-dlp `2023.01.02` or above.

You can install this package with pip:
```
python3 -m pip install -U https://github.com/sakura4919/yt-dlp-YTNSigDeno/archive/main.zip
```

See [yt-dlp installing plugins](https://github.com/yt-dlp/yt-dlp#installing-plugins) for the many other ways this plugin package can be installed.
