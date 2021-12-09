
# Install GAMS through flatpak

## Why ?

I use `guix` as a daily driver, GAMS' base installation doesn't work on such distributions, and packaging the app for `guix` would have been lengthy and inadapted.

GAMS being a proprietary application, the file just contains the yaml configuration file, **this is not a proper flatpak repository**, since it would need your specific`gamslice.txt` file in order to build properly.

## How To Use

### Dependencies

`flatpak-builder`, `libelf`

### Installation

- Add your GAMS license as the `gamslice.txt` file on the repo root directory.
- run `flatpak-builder --install build-dir org.flatpak.GAMS` to build the app in the `build-dir` directory
- Maybe you'll need to copy your `gamslice.txt` file in a directory such as `.var/app/org.flatpak.GAMS/data/gamslice.txt `

## Support

This is an incomplete repo, don't hesitate to interact through github or by email to enhance / debug it.

I have "post-installation" negligible errors on `guix`, but works correctly.

## License

MIT
