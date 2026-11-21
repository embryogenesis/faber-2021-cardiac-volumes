# Faber et al. 2021 — segmented AmiraMesh volumes, ten Carnegie stages

A **verbatim mirror** of [`10.6084/m9.figshare.13378742`](https://doi.org/10.6084/m9.figshare.13378742), redistributed under the terms of the licence the depositors chose. No file has been modified.

## Attribution

> Faber, Jan Willem; Hagoort, Jaco; Moorman, Antoon F. M.; Christoffels, Vincent M.; Jensen, Bjarke
>
> Faber JW, Hagoort J, Moorman AFM, Christoffels VM, Jensen B (2021). Quantified growth of the human embryonic heart. Biology Open.
>
> DOI: [10.6084/m9.figshare.13378742](https://doi.org/10.6084/m9.figshare.13378742) — licensed **CC BY 4.0**

Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); see [`LICENSE`](LICENSE). You may share and adapt this material for any purpose, including commercially, provided you give appropriate credit, link to the licence and indicate if changes were made. **This mirror makes no changes.**

## What this is

Labelled volumes for Carnegie stages 10, 11, 12, 13, 14, 15, 16, 18, 20 and 23, with an interactive 3D-PDF for each. The find that unblocked roadmap item 1: the only permissively licensed segmented Carnegie series this project has located. Cardiac-focused, which is a gift rather than a limitation — compact and trabecular myocardium are segmented separately, which is exactly the architecture behind the ventricular twist the atlas wants, and the heart is what its eight-parameter morph most conspicuously lacks.

## Provenance of the material

The depositors state that the specimens were left-over material from induced abortions on social indication at Tartu University Hospital, Estonia, collected with the permission of the relevant medical ethics committees, and that no informed consent was obtained for this particular re-use because the series had been published previously.

## Contents

30 file(s), 2217.1 MB total.

**8 of these exceed GitHub's 100 MB per-file limit** and are published as assets on the [latest release](../../releases/latest) rather than committed to the tree. The repository holds the manifest and the licence; the release holds the bytes. Fetch them with:

```sh
gh release download --repo embryogenesis/faber-2021-cardiac-volumes --dir data
```

| File | Size | SHA-256 |
| --- | --- | --- |
| `data/CS10-EMB-013-cTnI.am` _(release asset)_ | 207.1 MB | `ace99f0aca85deb7…` |
| `data/CS11-EMB-071-labels.am` | 8.8 MB | `218d2ba02f056297…` |
| `data/CS11-EMB-071-myomix.am` _(release asset)_ | 173.8 MB | `490cd36ac492765a…` |
| `data/CS12-EMB-054-labels.am` | 11.1 MB | `b1d5a66c8fa17d4d…` |
| `data/CS12-EMB-054-myomix.am` _(release asset)_ | 201.5 MB | `e29f21fa70578e40…` |
| `data/CS13-EMB-028-labels.am` | 5.8 MB | `0eb490983fb8002d…` |
| `data/CS13-EMB-028-myomix.am` _(release asset)_ | 268.7 MB | `30e264bce7e511fa…` |
| `data/CS14-EMB-026-cTnI.am` | 86.9 MB | `2b6bd46e78bbe478…` |
| `data/CS14-EMB-026-labels.am` | 7.1 MB | `186b73594667639a…` |
| `data/CS15-EMB-059-cTnI.am` | 82.5 MB | `f537eadce632d0f4…` |
| `data/CS15-EMB-059-labels.am` | 6.2 MB | `090906309c2deec8…` |
| `data/CS16-EMB-078-cTnI.am` _(release asset)_ | 173.3 MB | `aa5b85ac50142366…` |
| `data/CS16-EMB-078-labels.am` | 5.4 MB | `f2c8fc3449bd10cf…` |
| `data/CS18-EMB-006-cTnI.am` _(release asset)_ | 226.7 MB | `5d9e3447c6971602…` |
| `data/CS18-EMB-006-labels.am` | 17.9 MB | `5b07aa265a6ca1ab…` |
| `data/CS20-EMB-005-cTnI.am` _(release asset)_ | 323.3 MB | `4f4f08d1ca2c174c…` |
| `data/CS20-EMB-005-labels.am` | 8.6 MB | `2d27173adc5b7223…` |
| `data/CS23-EMB-084-cTnI.am` _(release asset)_ | 283.4 MB | `5f8e84cf3283f131…` |
| `data/CS23-EMB-084-labels.am` | 10.0 MB | `7376b2db5be7bec8…` |
| `data/CS10-EMB-013_labels.am` | 3.7 MB | `399c8bb6168ed2e4…` |
| `data/CS15-EMB-059.pdf` | 12.0 MB | `5f9c82eed420cbde…` |
| `data/CS16-EMB-078.pdf` | 11.9 MB | `60383bf91565a0fa…` |
| `data/CS18-EMB-006.pdf` | 12.0 MB | `743add84fc2975b8…` |
| `data/CS20-EMB-005.pdf` | 12.3 MB | `cea29edd0b7dfdd0…` |
| `data/CS23-EMB-084.pdf` | 12.1 MB | `297a9ecb0260d908…` |
| `data/CS10-EMB-013.pdf` | 7.5 MB | `6f85efa81e2d8734…` |
| `data/CS11-EMB-071.pdf` | 7.5 MB | `9affb4d0ed57c48d…` |
| `data/CS12-EMB-054.pdf` | 7.7 MB | `cab0ddc201ee80ed…` |
| `data/CS13-EMB-028.pdf` | 10.7 MB | `57ee938813effe28…` |
| `data/CS14-EMB-026.pdf` | 11.3 MB | `51f1285b00ab5246…` |

Full checksums, original filenames and the source article id for every file are in [`MANIFEST.json`](MANIFEST.json).

(22 smaller file(s) are committed normally.)

## Notes for anyone using this

- Format is AmiraMesh: an ASCII header (`# AmiraMesh BINARY-LITTLE-ENDIAN 2.1`) followed by one byte per voxel. Documented and trivially parsed, unlike anything else in this space.
- The CS13 label file names 25 real anatomical structures; the remaining ~195 entries are per-slice registration markers rather than anatomy. Do not treat the label count as a structure count.
- Eight of the thirty files exceed GitHub's 100 MB hard limit, from 173 MB to 323 MB, so those ship as Release assets rather than in the tree; the other 22 are committed normally. See README.
- Grid for CS13 is 1372 x 1020 x 192. Expect ~270 MB per uncompressed volume.

## Verifying the mirror

```sh
# every file, against the manifest
python3 -c "import json,hashlib,pathlib;m=json.load(open('MANIFEST.json'));[print(('ok  ' if hashlib.sha256(pathlib.Path(f['path']).read_bytes()).hexdigest()==f['sha256'] else 'BAD ')+f['path']) for f in m['files'] if pathlib.Path(f['path']).exists()]"
```

---

Mirrored 2026-11-21 by `tools/mirror.ts` in the atlas repository, which re-verifies the licence of every article against the live Figshare metadata before downloading anything and aborts on a mismatch.
