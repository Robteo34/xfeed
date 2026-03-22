# 𝕏 Analyst Feed — Market Intel

Aplikacja do pobierania tweetów analityków krypto w czasie rzeczywistym przez Vercel + RapidAPI.

## Struktura

```
xfeed-github/
├── api/tweets.js        ← backend proxy (Vercel serverless)
├── public/index.html    ← frontend (mobile PWA)
├── vercel.json          ← konfiguracja Vercel
└── README.md
```

## Deploy krok po kroku

### 1. GitHub
1. github.com → "New repository" → nazwa: `xfeed`
2. Wgraj te 4 pliki zachowując strukturę folderów

### 2. Vercel
1. vercel.com → zaloguj przez GitHub
2. "Add New Project" → wybierz repo `xfeed` → Deploy

### 3. Klucz API
1. Projekt → Settings → Environment Variables
2. Dodaj: Name = `RAPIDAPI_KEY` | Value = Twój klucz z rapidapi.com (twitter241)
3. Deployments → Redeploy

### 4. Użycie
1. Skopiuj URL projektu (np. `https://xfeed-abc.vercel.app`)
2. Otwórz w przeglądarce telefonu
3. Wklej URL w pole konfiguracji
4. Kliknij "POBIERZ TWEETY"

### 5. Dodaj do ekranu głównego
- **iPhone**: Safari → ikona Share → "Dodaj do ekranu głównego"
- **Android**: Chrome → ⋮ → "Dodaj do ekranu głównego"

## Monitorowane konta (12)
@paweljezowski @marekmeissner @mastemindzx @HsakaTrades
@CryptoHayes @woonomic @nic__carter @hasufl
@RaoulGMI @DylanLeClair_ @MessariCrypto @glassnode

## Połączenie z botem
Po deploymencie wklej URL serwera w zakładkę "𝕏 X Feed" w głównym bocie (signal-bot-v5).
Bot automatycznie przełączy się z AI feed na prawdziwe tweety.
