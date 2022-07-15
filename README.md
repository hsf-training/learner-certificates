# Certificates for The Carpentries

This repository generates certificates for participants.

## Pure python method

### Install required packages

```
pip3 install jinja jinja2-cli svglib
```

### Generate certificate

```
jinja2 swc-hsf-iris-hep-attendance.svg -D name="Firstname Lastname" -D date="Nov. 6, 2022" -D instructor="Some Instructor Name" > generated_certificate.svg && svg2pdf generated_certificate.svg
```

The certificate is now available as `generated_certificate.pdf`.

## Alternative method with cairosvg

This depends ont he python package cairosvg which in turn depends on cairo development libraries being installed. To use this method, use `bin/certificates.py` to build certificates.


