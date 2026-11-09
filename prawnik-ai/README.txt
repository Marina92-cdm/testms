PRAWNIK AI — przegląd umów / contract review

URUCHOMIENIE
1. Rozpakuj cały ZIP.
2. Wymagany Python 3 (https://www.python.org/downloads/).
3. Mac: uruchom Start-Mac.command. Windows: Start-Windows.bat.
   Alternatywnie otwórz terminal w tym folderze: python3 start.py
4. Przeglądarka otworzy aplikację. Pozostaw okno serwera otwarte.
   Zakończenie: Ctrl+C w oknie serwera.
Nie otwieraj samego index.html dla lokalnego AI: potrzebny jest lokalny serwer.
Możesz też umieścić index.html, app.js i style.css na hostingu HTTPS.

UŻYWANIE
Wczytaj przykład umowy po angielsku, wklej tekst lub dodaj plik DOCX / TXT.
Word DOCX jest importowany lokalnie. Starszy DOC zapisz w Wordzie jako DOCX.
PDF nie jest importowany: skopiuj tekst i wklej do pola.
Import Worda odczytuje tekst główny, bez pełnego układu dokumentu.
Porównaj wynik z oryginałem; komentarze, przypisy, nagłówki i zmiany mogą zostać pominięte.
Limit: 60 000 znaków, plik DOCX do 10 MB, TXT do 1 MB.
Wybierz język umowy (English lub Polski), rolę oraz kontekst.
Dla umowy angielskiej wybierz "Inny / nieznany", jeśli nie podlega prawu polskiemu.

DWA TRYBY — BEZ KLUCZA API
• Szybki przegląd regułami: wykrywa wybrane frazy w języku polskim lub angielskim.
  To nie jest AI. Wskazuje kategorię raz, z pierwszym pasującym akapitem.
  Wybrana rola i kontekst są zapisane w raporcie, ale nie zmieniają reguł.
• Lokalne AI: WebLLM i model Qwen2.5 1.5B. Pierwsze uruchomienie pobiera
  około 1 GB danych. Wymaga internetu do pobrania, obsługi WebGPU,
  odpowiedniej pamięci i sprzętu. Użyj aktualnej przeglądarki z WebGPU.
  AI uwzględnia wybraną rolę i kontekst; wynik w języku wybranym w formularzu.
  Długie dokumenty są analizowane w częściach, bez pełnej oceny zależności.
  Model jest mały i nie jest wyspecjalizowanym ani zweryfikowanym prawnikiem.
  Nie udało się zweryfikować uruchomienia modelu AI na urządzeniu autora paczki.
  W razie błędu pobierania lub zgodności skorzystaj z trybu reguł.

PRYWATNOŚĆ I OGRANICZENIA
Aplikacja nie wysyła tekstu umowy do serwera analizy. Tekst i wynik są
przechowywane w pamięci strony; odświeżenie je usuwa. Zewnętrzne usługi
CDN, Google Fonts i Hugging Face otrzymują typowe dane połączenia podczas
pobierania zasobów. Model może pozostać w cache przeglądarki.
Nie ma kont użytkowników ani trwałej historii. Pobierz wynik jako TXT.

Żaden tryb nie gwarantuje wykrycia wszystkich ryzyk. Nie weryfikuje aktualnego
prawa, orzecznictwa ani skuteczności klauzul. Wnioski i proponowane zmiany
wymagają sprawdzenia przez prawnika właściwej jurysdykcji.

ENGLISH QUICK START
Extract the ZIP. Install Python 3 if needed. Run start.py with Python 3;
the app opens on a local address. Keep the terminal open.
The interface is Polish. Select English for English-language contract findings.
Load the English example or paste/import a DOCX or TXT contract. Choose rules (no AI)
or local AI (WebGPU and roughly 1 GB download, no API key).
Neither mode is a legal opinion or a guarantee of complete risk detection.

REFERENCE
WebLLM: https://webllm.mlc.ai/docs/user/get_started.html
