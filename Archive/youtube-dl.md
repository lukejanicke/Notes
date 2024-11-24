# youtube-dl

- [youtube-dl](https://github.com/ytdl-org/youtube-dl)

## Installation

Install with [Homebrew](Homebrew.md).

```zsh
brew install youtube-dl
```

## Examples

```zsh
youtube-dl [OptionS] "URL" [URL...]
```

List all available formats.

```zsh
youtube-dl -F "URL"
```

Download video with specified format.

```zsh
youtube-dl -f FORMAT "URL"
```

Download video with all available subtitles.

```zsh
youtube-dl -f FORMAT --all-subs "URL"
```

List available subtitle languages and formats.

```zsh
youtube-dl --list-subs "URL"
```

Download video with subtitles in specified language and format.

```zsh
youtube-dl -f FORMAT --sub-lang LANGS --sub-format FORMAT "URL"
```

Download video with subtitles embedded. [FFmpeg](FFmpeg.md) required.

```zsh
youtube-dl -f FORMAT --embed-subs --all-subs "URL"
```

Download videos from URLs in a file with `-a FILE` or `--batch-file FILE`.

```zsh
youtube-dl [OptionS] -a FILE
```

## Configuration

Save default configurations in `~/.config/youtube-dl/config`.
