# Wercker Base Box

This container image is intended to be used as a general purpose base box for Wercker Pipelines. Based on `debian:stable-slim` with additional generic packages.

## Usage

Include the box definition either for all pipelines in the `wercker.yml` as follows:

    box: jappievw/wercker-box-base
    
    build:
      steps:
        - script:
            code: |
              echo "Foo bar"

Or as a specific box for a single pipeline as follows:

    build:
      box: jappievw/wercker-box-base
      steps:
        - script:
            code: |
              echo "Foo bar"
