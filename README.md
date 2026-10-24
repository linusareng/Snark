# Snark

A marker-hand display typeface by Linus Areng. One weight, Latin.

![Specimen](documentation/specimen.png)

## Building

```sh
python3 -m venv venv && source venv/bin/activate
pip install gftools fontmake fontbakery shaperglot

cd sources && gftools builder config.yaml
```

Output lands in `fonts/ttf/`. CI runs the same build plus FontBakery on every push.

## Source

`sources/Snark.glyphs` is the canonical source — build from it, not from the
compiled binaries. Vertical metrics, `fsType` and the OFL name records are set
as Glyphs custom parameters so they survive rebuilds.

## License

[SIL Open Font License 1.1](OFL.txt). No Reserved Font Name.
