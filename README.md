# Hörpusýn Myndavélahönnuður

Kerfishönnuður og verðreiknir fyrir [Hörpusýn](https://blaberg.is) myndavélakerfi frá Bláberg.

Notendur geta valið fjölda myndavéla, staðsetningar, áskriftarleiðir og viðbætur — og fengið verðáætlun samstundis.

## Keyrsla staðbundið

Opnaðu `index.html` beint í vafra — engin build-skref eða pakkastjóri þarf.

## Deploy á Google Cloud App Engine

```bash
gcloud app deploy --quiet --project=<PROJECT_ID>
```

## Tengd Repo

| Repo | Lýsing |
|------|--------|
| [Blaberg-Horpusyn](https://github.com/snoste/Blaberg-Horpusyn) | Edge node BalenaOS forritið (backend, frontend, Frigate, MediaMTX) |

## Skráaryfirlit

| Skrá | Lýsing |
|------|--------|
| `index.html` | Aðalsíðan — hönnuður, verðreiknir og kynning |
| `app.yaml` | Google Cloud App Engine stillingar |
| `camera.webp` / `camera_hero.png` | Myndir af Hörpusýn myndavélum |
| `preview-blaberg.html` | Forskoðunarsíða |

---

© 2026 Bláberg ehf.
