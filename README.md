# texttospeech

## PREREQUISITES

* ffplay installed
* ~/.local folder wired properly (tested on Ubuntu 18.04)

## INSTALL

    usage: ./install --install [google_cloud_key_json_file]
    
    Arguments
      google_cloud_key_json_file  google cloud json file path
                                  (optional if already installed)

## USAGE

    usage:
      texttospeech [-fa] <text>  convert text to speech and play
                                 (-f to overwrite locally cached file,
                                  -a to run asynchronously)
      texttospeech --list|-l     ls mp3 folder
      texttospeech --clean       remove mp3 files

## SETUP GIT

    ./setup_git

    # setup_git content:
    #!/bin/bash
    
    cat <<EOF > .git/hooks/pre-commit
    ./docgen
    git add README.md
    EOF
    
    chmod +x .git/hooks/pre-commit

## LICENSE

MIT License

Copyright (c) 2020 Jan Święcki

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
