# Manim

- [manim](https://github.com/3b1b/manim)

## Dependencies

Install dependencies with [Homebrew](Homebrew.md).

```zsh
brew install cairo
brew install sox
brew install ffmpeg
```

`pkg-config` is possibly not required.

```zsh
brew install pkg-config
```

Install the full [MacTeX](https://tug.org/mactex/) distribution why not. Fetch a 🍺 and wait.

```zsh
brew cask install mactex
```

## Python virtual environment

Install with [Python](Python.md).

```zsh
cd ~/Development
mkdir manim
python3 -m venv manim
cd manim
source bin/activate
```

Manually install the Python packages that Manim needs.

Use the virtual environment’s `pip` here.

```zsh
pip install colour data decorator ffmpeg funcsigs future latex numpy opencv-python Pillow progressbar pycairo pydub scipy shutilwhich six sox tempdir tqdm
```

Confirm that all required packages are present.

```zsh
pip freeze
```

`pygments` also appears to be needed.

```zsh
pip install pygments
```

## Manim

Stay in ``~/Development/manim` with the virtual environment active.

```zsh
git clone https://github.com/3b1b/manim.git
```

Open `manim/manimlib/constants.py` and edit line 26., change `Media_Dir` to desired media output location.

**Current**

```
"Dropbox (3Blue1Brown)/3Blue1Brown Team Folder"
```

**Example**

```
"Development/manim/output"
```

Start manim.

```zsh
cd manim
python manim.py example_scenes.py
```
