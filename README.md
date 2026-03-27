# Bláberg Hönnuðir

Kerfishönnuðir og verðreiknar fyrir öryggis- og myndavélakerfi frá [Bláberg](https://blaberg.is).

## Hönnuðir

| Hönnuður | URL | Mappa | Lýsing |
|----------|-----|-------|--------|
| **Myndavélar** | [myndavelar.blaberg.is](https://myndavelar.blaberg.is) | `myndavelar/` | Hörpusýn myndavélakerfi — AI-greining, fjaraðgangur |
| **Öryggiskerfi** | [kerfi.blaberg.is](https://kerfi.blaberg.is) | `kerfi/` | Chuango öryggiskerfi — skynjurar, viðvaranir, þjónustusamningar |

## Keyrsla staðbundið

Opnaðu `myndavelar/index.html` eða `kerfi/index.html` beint í vafra — engin build-skref þarf.

## Deploy á Google Cloud

```bash
# Myndavélar (myndavelar.blaberg.is)
cd myndavelar && gcloud run deploy myndavelar-designer --source . --region europe-west1 --allow-unauthenticated

# Öryggiskerfi (kerfi.blaberg.is)
cd kerfi && gcloud run deploy kerfi-designer --source . --region europe-west1 --allow-unauthenticated
```

## Tengd Repo

| Repo | Lýsing |
|------|--------|
| [Blaberg-Horpusyn](https://github.com/snoste/Blaberg-Horpusyn) | Edge node BalenaOS forritið (backend, frontend, Frigate, MediaMTX) |

## Skráaryfirlit

```
├── myndavelar/           # Hörpusýn myndavélahönnuður
│   ├── index.html        # Aðalsíða
│   ├── Dockerfile        # Cloud Run deployment
│   ├── app.yaml          # App Engine stillingar
│   ├── camera.webp       # Myndavélarmynd
│   ├── camera_hero.png   # Hero mynd
│   └── preview-blaberg.html
├── kerfi/                # Öryggiskerfishönnuður
│   ├── index.html        # Aðalsíða
│   ├── Dockerfile        # Cloud Run deployment
│   └── app.yaml          # App Engine stillingar
└── README.md
```

---

© 2026 Bláberg ehf.
