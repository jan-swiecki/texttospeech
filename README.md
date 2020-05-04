# texttospeech

## INSTALL

    usage: ./install <google_cloud_key_json_file>

## USAGE

    usage:
      texttospeech [-f] <text>  convert text to speech
                                (-f to overwrite locally cached file)
      texttospeech --list|-l    ls mp3 folder
      texttospeech --clean      remove mp3 files

## SETUP GIT

    # setup_git content
    #!/bin/bash
    
    cat <<EOF > .git/hooks/pre-commit
    ./docgen
    git add README.md
    EOF
    
    chmod +x .git/hooks/pre-commit
