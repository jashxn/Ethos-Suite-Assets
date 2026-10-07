# Bundled text fonts

These files are original static TrueType fonts from pinned upstream commits. They are distributed under SIL Open Font License 1.1 with the original copyright and license notices. Keep each family's notices with its font files when publishing or redistributing this directory.

| Family | Original version | Normal weights | Italic weights | Files |
| --- | --- | --- | --- | --- |
| Geist | 1.800 | 100–900, steps of 100 | 100–900, steps of 100 | 18 |
| Cal Sans | 2.010 | 400, 500, 600, 700 | 400, 500, 600, 700 | 8 |
| Manrope | 4.505 | 200–800, steps of 100 | None | 7 |
| Space Grotesk | 2.000 | 300, 400, 500, 700 | None | 4 |

The 37 TTF files total 5,601,564 bytes. No files were converted, subsetted, renamed, or instantiated from a variable font. All faces are static fonts with `OS/2.fsType = 0`. The face list records only weights and styles present in the source files; it does not invent missing bold or italic faces.

## Sources

- [Geist source](https://github.com/vercel/geist-font/tree/10dc7658f13c38a474cde201bb09a4617267545b): `fonts/Geist/ttf`. The upstream `OFL.txt`, `LICENSE.txt`, `AUTHORS.txt`, and `CONTRIBUTORS.txt` are included unchanged.
- [Cal Sans source](https://github.com/calcom/sans/tree/b0d806d61b3430e58e7f87465b9c1e1e72544033): `fonts/calsans-static-base/CalSans-*.ttf`. This is the base Cal Sans family. The upstream `OFL.txt`, `AUTHORS.txt`, and `CONTRIBUTORS.txt` are included unchanged.
- [Manrope source](https://github.com/googlefonts/manrope/tree/468c0dbe38efa331b80bfe9448256abe27be44c3): `fonts/ttf`. The upstream `OFL.txt` is included unchanged. These are the OFL-licensed 4.505 files, not the separately licensed V5 files on the [designer's website](https://www.sharanda.com/manrope).
- [Space Grotesk source](https://github.com/floriankarsten/space-grotesk/tree/03507d024a01282884232081fc6011c09ff4e849): `fonts/ttf/static`. The upstream `OFL.txt`, `AUTHORS.txt`, and `CONTRIBUTORS.txt` are included unchanged. This pinned source has no static 600 face or italic faces.

## Manifest and publication

`manifest.json` records each family's repository, immutable source revision, OFL notice, and original notice files. Each face records its relative path, immutable source URL, Git blob SHA, byte count, SHA-256, Adler-32 checksum, weight, style, internal names, version, and embedding flag. Adler-32 uses eight lowercase hexadecimal characters and is the checksum consumed by the client asset loader.

Every downloaded file was checked against the source Git tree's byte count and blob SHA. The TrueType name, OS/2, and table directory records were read to verify each face. These static checks do not establish native client rendering results.

Publish the family directories, this README, `.gitattributes`, `license-review.json`, and `manifest.json` together. Use an immutable published commit in client URLs. Keep the original notice bytes, including their line endings. Font payloads remain lazy client downloads; this directory does not execute remote code or load fonts on import.

## Requested fonts not included

Satoshi is not included. The [official ITF Free Font License](https://www.fontshare.com/licenses/itf-ffl), Version 2.0 dated 17 August 2026, permits some use in the licensee's own applications but restricts redistribution through repositories and font libraries. It also restricts making fonts selectable by third-party users. Fontshare identifies Satoshi as `itf_ffl`. Publishing its raw files in a public assets repository or shipping them as a library font requires separate distribution rights. The official page's [application script](https://www.fontshare.com/js/main.d962d2d8.js) contains the license text; it was inspected without executing it on 7 October 2026.

Aeonik and Helvetica are also excluded pending suitable redistribution and application embedding rights. Do not add trial files, system-installed files, third-party mirror copies, or substitute files bearing these family names. `license-review.json` records the exclusion status; it is not a license grant.
