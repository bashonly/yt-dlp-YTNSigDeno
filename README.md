> [!CAUTION]
> ### This plugin is obsolete as of yt-dlp version `2025.11.11`.
>
> **The plugin is completely unrelated to yt-dlp's built-in Deno support.**
>
> **Please uninstall the plugin**, and refer to https://github.com/yt-dlp/yt-dlp/wiki/EJS for guidance on yt-dlp's native Deno support.

---

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

Requires yt-dlp `2024.12.06` or above.

You can download the wheel of the [latest release](https://github.com/bashonly/yt-dlp-YTNSigDeno/releases/latest) and place the `.whl` file in one of [yt-dlp's plugin paths](https://github.com/yt-dlp/yt-dlp#installing-plugins).

Or you can install this package with pip:
```
python3 -m pip install -U https://github.com/bashonly/yt-dlp-YTNSigDeno/archive/master.zip
```

See [the plugins section of the yt-dlp README](https://github.com/yt-dlp/yt-dlp#installing-plugins) for more information.
