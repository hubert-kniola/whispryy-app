# Whispryy — napisy na żywo

Whispryy zamienia rozmowę z kanału głosowego Discorda — albo dźwięk z przeglądarki czy innego programu —
na **napisy na żywo, wprost na ekranie gry**. Pokazuje, kto mówi, a mowa jest rozpoznawana **lokalnie,
na Twoim komputerze**: dźwięk nigdzie nie jest wysyłany.

Stworzone z myślą o osobach głuchych i słabosłyszących, przydaje się też w hałasie, w nocy czy przy słabym audio.

**🌐 Strona:** https://hubert-kniola.github.io/whispryy-app/

## ⬇ Pobierz

### [Pobierz Whispryy dla Windows](https://github.com/hubert-kniola/whispryy-app/releases/latest/download/Whispryy.zip)

Windows 10/11 64-bit · jedna wersja dla kart NVIDIA, AMD i Intel · [wszystkie wersje](https://github.com/hubert-kniola/whispryy-app/releases)

## Co potrafi

- **Słyszy tylko wybrany program** — Discorda, przeglądarkę albo dowolny inny program. Gra, muzyka
  i inne aplikacje nie trafiają do napisów.
- **Pokazuje, kto mówi** — przy Discordzie każda osoba ma na napisach własny kolor nicku.
- **Napisy tam, gdzie chcesz** — w dowolnym rogu albo w wybranym miejscu ekranu; skrót klawiszowy
  (domyślnie `Ctrl+Alt+N`) przełącza położenie także w czasie gry.
- **Dopasujesz wygląd** — czcionka, szerokość, przezroczystość, czas wyświetlania.
- **Nie przeszkadza w grze** — zostawia grze część procesora i pamięci karty graficznej.
- **Prywatność** — rozpoznawanie mowy działa na Twojej karcie graficznej, bez wysyłania dźwięku do internetu.
- **Aktualizuje się samo** — informuje o nowej wersji, instalujesz jednym kliknięciem.

## Instalacja

1. Pobierz `Whispryy.zip` i **rozpakuj cały folder**, np. na Pulpit albo do Dokumentów.
   Nie rozpakowuj do *Program Files* i nie uruchamiaj prosto z ZIP-a.
2. Uruchom `Whispryy.exe`. Jeśli Windows pokaże „System Windows ochronił komputer”, kliknij
   **Więcej informacji → Uruchom mimo to** (program nie ma płatnego podpisu cyfrowego).
3. Przy pierwszym uruchomieniu Whispryy pobierze model rozpoznawania mowy (~1,6 GB), a na kartach NVIDIA
   także biblioteki CUDA (~1,2 GB). Postęp — z procentami — widać w panelu, na stronie **Stan**.
   Robi się to tylko raz.

Whispryy działa w tle — ikona jest w zasobniku obok zegara. Kliknij ją, żeby otworzyć panel.

## Wymagania

- Windows 10 lub 11, 64-bit.
- Karta graficzna z aktualnymi sterownikami: **NVIDIA** (GeForce / RTX), **AMD Radeon** albo **Intel Arc**.
  Whispryy sam wybiera, na czym działać.
- Bez dedykowanej karty działa na procesorze — wolniej i mniejszym modelem.
- Ok. 5 GB wolnego miejsca na dysku (program, model i — na kartach NVIDIA — biblioteki CUDA).

## Aktualizacje

Whispryy sam sprawdza, czy jest nowa wersja, i pokazuje powiadomienie. Instalujesz ją jednym kliknięciem
w panelu, w zakładce **Aktualizacje** — program uruchomi się ponownie. Ustawienia, klucze Discorda
i pobrany model zostają.

## Nicki i „kto mówi” (opcjonalnie, ok. 2 minut)

Napisy działają od razu. Żeby widzieć też, kto mówi, połącz Whispryy z Discordem — instrukcja krok po kroku
jest w panelu, w zakładce **Discord**:

1. Utwórz darmową aplikację w [Discord Developer Portal](https://discord.com/developers/applications) (**New Application**).
2. W zakładce **OAuth2** skopiuj **Client ID** i **Client Secret** (**Reset Secret**).
3. W **Redirects** dodaj `http://localhost` i kliknij **Save Changes**.
4. Wklej klucze w panelu Whispryy → **Zapisz i połącz** → w Discordzie kliknij **Autoryzuj**.

## Pytania i problemy

- **Czy mój dźwięk jest wysyłany do internetu?** Nie. Mowa jest rozpoznawana na Twoim komputerze.
- **Nie widzę napisów własnego głosu.** Discord nie odtwarza Twojego mikrofonu, więc Whispryy go nie słyszy.
- **Napisy nie pokazują się w grze.** Gry w trybie pełnoekranowym wyłącznym zasłaniają napisy — przełącz grę
  na tryb okna bez ramki (*borderless*).
- **Ciche osoby są pomijane.** W panelu, na stronie **Stan**, obniż **Próg mowy**.
- **Aktualizacja się nie instaluje.** Folder Whispryy musi mieć prawo zapisu — przenieś go np. do Dokumentów.
- **Coś nie działa?** Panel → **Ogólne** → **Log błędów** — ten plik pomoże znaleźć przyczynę.
  Problem możesz zgłosić w [Issues](https://github.com/hubert-kniola/whispryy-app/issues).

Ustawienia i logi są w `%APPDATA%\Whispryy`.

---

## English

**Whispryy** turns Discord voice chat — or audio from a browser or any other app — into **live captions on top
of your game**, shows who is speaking, and recognizes speech **locally on your PC** (your audio is never uploaded).

**[Download for Windows](https://github.com/hubert-kniola/whispryy-app/releases/latest/download/Whispryy.zip)**
(Windows 10/11 64-bit; NVIDIA, AMD or Intel GPU) · [Website](https://hubert-kniola.github.io/whispryy-app/)

Unzip the whole folder (e.g. to the Desktop, not *Program Files*) and run `Whispryy.exe`. On first launch it
downloads the speech model (and CUDA libraries on NVIDIA cards). Updates install with one click
from the **Aktualizacje** (Updates) tab. The app interface is in Polish.

---

<sub>To repozytorium zawiera tylko wydania i stronę — kod źródłowy aplikacji nie jest publiczny.</sub>
