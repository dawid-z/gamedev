# Game Dev

### 1. Porównanie Generatorów 3D AI

| Narzędzie | Geometria (Detale) | Tekstury | Zastosowanie | Cena (orientacyjna) | **Licencja / Uwagi prawne** |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Tripo AI Ultra** | **Najlepsza (organiczne)**, dużo mikro-detali. | Najbardziej naturalne, szczegółowe. | Postacie, kształty organiczne. | ~$20/mies. | **Pełne prawa komercyjne** (w płatnym planie). |
| **Hunyuan 3D 3.0** | Dobre krawędzie (hard surface), gubi detale twarzy. | Czyste, techniczne, słabsze przy twarzach. | Maszyny, obiekty techniczne. | Darmowy (limitowany). | ⚠️ **Restrykcyjna / Niejasna**. Modele mogą należeć do Tencent; zalecana ostrożność (użytek niekomercyjny). |
| **Hitem3D 1.5** | Dobre krawędzie (hard surface). | Wysoki kontrast, czasem przesycone. | Obiekty twarde, wysoka jakość. | Najdroższa opcja (kredyty). | **Komercyjna** (płacisz za każdy model/kredyty). |
| **Meshy 6** | Problemy z proporcjami przy organice. | Przeciętne w tym zestawieniu. | Ogólne zastosowanie. | Subskrypcja SaaS. | **Komercyjna** (w ramach subskrypcji). |

---

### 2. Tier List Silników Gier

| Tier | Silnik | Główne Zalety | Główne Wady | Dla kogo? | **Model Finansowy / Licencja** |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **S** | **Unreal Engine** | Grafika (Nanite/Lumen), Blueprints. | Wymagający sprzętowo, trudniejszy C++. | Indie i AAA. | **Royalty**: Darmowy do 1 mln USD przychodu, potem 5%. |
| **A** | **Unity** | Wszechstronność, C#, baza wiedzy. | Bałagan w renderowaniu, reputacja. | Mobile, 2D/3D. | **Seat**: Darmowy do progu (Personal), potem płatny za stanowisko. |
| **A** | **Godot** | Lekki, Open Source. | Mniej hitów, mniejszy rynek pracy. | Indie, 2D/3D. | **100% Free**: Licencja MIT, brak opłat i royalty. |
| **A/B**| **RPG Maker** | Łatwy, bez kodowania. | Ograniczony do jednego gatunku. | Pisarze, RPG 2D. | **Jednorazowy zakup**: Płacisz raz, masz prawa komercyjne. |
| **C** | **Game Maker** | Prosty start w 2D. | Opłaty nawet bez sukcesu. | Początkujący. | **Subskrypcja**: Wymagana miesięczna opłata, by eksportować grę. |
| **C** | **Phaser** | HTML5/JS, lekki. | Tylko webowe. | Game Jamy. | **100% Free**: Open Source. |
| **D** | **CryEngine** | Grafika. | Brak dokumentacji, trudny. | Duże studia. | **Royalty**: 5% prowizji po przekroczeniu 5000 USD przychodu. |
| **F** | **Construct 3** | Visual scripting. | Drogi, JS. | Unikać. | **Subskrypcja**: Płatny miesięcznie, darmowa wersja bardzo okrojona. |

---

### 3. Unreal Engine Tips

#### 1. Edytor, UI i Praca na Plikach
| Skrót / Funkcja | Opis |
| :--- | :--- |
| **Property Matrix** | Masowa edycja właściwości wielu zaznaczonych assetów. |
| **Unhide Runtime Components** | W "Editor Preferences" odznacz ukrywanie komponentów dodanych przez Construction Script. |
| **Launch with -basedir** | Uruchom build (Shipping) z lokalnego .exe używając flagi `-basedir` do folderu projektu. |
| **Global User Config** | Pliki .ini w `AppData` nadpisują ustawienia dla wszystkich projektów UE na dysku. |
| **Solution Name from Folder** | Wymuś nazwę pliku `.sln` zgodną z nazwą folderu (przydatne przy branchach). |
| **Widget Reflector** | Skalowanie interfejsu edytora (Application Scale). |
| **Input Visualization** | Wizualizacja kliknięć i klawiszy na ekranie (w Widget Reflector). |
| **Disable Tooltips** | Wyłączenie dymków podpowiedzi (dobre do nagrywania wideo). |
| **F10 / Ctrl+Shift+T** | Zwiększenie obszaru roboczego (ukrycie paneli / paska narzędzi). |
| **Actor Palette** | Plugin pozwalający używać poziomu jako palety drag & drop. |
| **Graph Zoom** | Przytrzymaj Ctrl podczas scrollowania, aby przybliżyć grafy bardziej niż zwykle. |
| **Copy as Text** | Assety i nody to tekst – możesz je wysłać komunikatorem i wkleić u siebie. |
| **Launch .uproject** | PPM na plik projektu -> "Launch Game" (szybki test bez edytora). |
| **Clean Default Root** | Przeciągnij nowy Scene Component na root, by usunąć "kulkę" billboardu. |
| **Reload Asset** | Przywraca asset do stanu z dysku (bez restartu edytora). |
| **Autosaves** | Przywracanie pracy z folderu `Saved/Autosaves`. |
| **Ctrl+Shift+N** | Utwórz nowy folder. |
| **F2** | Zmień nazwę (Rename). |
| **Shift+F2** | Masowa zmiana nazw zaznaczonych plików (Batch Rename). |
| **FOV Control** | PPM + C (zoom in) / Z (zoom out) zmienia kąt widzenia w Viewporcie. |
| **Ctrl+P** | Szybkie wyszukiwanie assetów (Quick Open). |
| **Copy Properties** | PPM na nazwę zmiennej -> Copy, Shift+LPM -> Paste. |
| **Ctrl+E** | Otwórz edytor dla zaznaczonego assetu. |
| **Shift+E** | Zaznacz wszystkich aktorów tej samej klasy na poziomie. |
| **Ctrl+B** | Znajdź asset w Content Browser (Browse to Asset). |
| **-newconsole** | Uruchom grę z osobnym oknem konsoli (zamknięcie okna zabija proces). |
| **Search Code for UI** | Szukaj tekstu błędu w kodzie źródłowym silnika (Github/Local). |
| **BugItGo** | Generuje komendę teleportującą do widoku kamery (do zgłaszania błędów). |
| **Thumbnail Edit Mode** | Edycja kąta kamery na miniaturkach assetów. |
| **Light Rotate (L+LPM)** | Obracanie światła w podglądzie assetu (Static Mesh/Material). |
| **Folder Filters** | Filtrowanie widoku tylko do konkretnego folderu w drzewie. |
| **Bookmarks (Ctrl+Tab)** | Zarządzanie zakładkami okien i szybkie przełączanie. |
| **Hide Library** | Ukrycie biblioteki gier w Epic Launcher. |
| **Classic Toolbar** | Komenda przywracająca stary wygląd paska narzędzi (UE4 style). |
| **Temp Pivot (Alt+MMB)** | Tymczasowe przesunięcie pivota obiektu. |
| **Material Param Shortcut** | Przypisz skrót klawiszowy do "Convert to Parameter". |
| **Console Var Help (?)** | Wpisz `[zmienna] ?` by dostać opis co ona robi. |
| **Plugin Ref Viewer** | Graf zależności między pluginami. |
| **Translucent Select (T)** | Klawisz T przełącza możliwość klikania obiektów przezroczystych. |
| **Python Startup** | Skrypty `init_unreal.py` uruchamiają się przy starcie edytora. |

#### 2. Blueprinty (Visual Scripting)
| Skrót / Funkcja | Opis |
| :--- | :--- |
| **Ctrl/Alt + Drag** | Przeciągnij zmienną z Ctrl (Get) lub Alt (Set). |
| **Auto Function Inputs** | Przeciągnij zmienną na węzeł "Entry", by dodać parametr. |
| **Format Text** | Użyj `{nazwa}` w tekście, by stworzyć piny (lepsze niż Append). |
| **Print Text Key** | Użyj klucza (Key), by nadpisywać jedną wiadomość na ekranie (zamiast spamu). |
| **Palette Window** | Lista wszystkich dostępnych nodów w panelu bocznym. |
| **Blueprint Debugger** | Narzędzie do śledzenia przepływu danych. |
| **Diff Blueprints** | Porównywanie zmian wizualnych między wersjami pliku. |
| **Align Nodes** | Shift + W/A/S/D (wyrównanie), Q (prostowanie linii). |
| **Validated Get** | Zamiana zwykłego Get na wersję z `IsValid` (PPM). |
| **BlueprintUpdateCamera** | Nadpisywanie logiki kamery w PlayerCameraManager. |
| **Disable Node** | Wyłączenie noda bez usuwania go (przepuszcza sygnał dalej). |
| **Shift+Delete** | Usuń noda, ale połącz piny wejścia z wyjściem. |
| **Math Expression Node** | Pisanie wzorów matematycznych (np. `(A+B)*2`) tworzy graf. |
| **Set Members in Struct** | Zmiana wybranych pól struktury bez rozbijania całości. |
| **Local Input Vars** | Dostęp do parametrów wejściowych funkcji jako zmiennych lokalnych. |
| **Recompile during PIE** | Możliwość kompilacji BP w trakcie gry (wymaga ustawienia w Project Settings). |
| **Break on Exceptions** | Pauza gry w momencie błędu Blueprinta. |
| **ExpandBoolAsExecs** | (C++) Zmienia bool return na dwa wyjścia Exec (True/False). |
| **DefaultToSelf** | (C++) Ukrywa pin, domyślnie przypisując `self`. |
| **Math in Fields** | Pola numeryczne obsługują proste równania matematyczne. |
| **Timer For Next Tick** | Wykonaj akcję w następnej klatce. |
| **Call in Editor (Seq)** | Wywoływanie funkcji BP przez Sequencer przy zmianie zmiennej. |

#### 3. Optymalizacja i Debugowanie
| Skrót / Funkcja | Opis |
| :--- | :--- |
| **Simple as Complex** | Użyj prostej kolizji jako dokładnej (oszczędność pamięci/CPU). |
| **Async Physics Tick** | Przesunięcie symulacji fizyki na inny moment klatki. |
| **Chaos Visual Debugger** | Nagrywanie i debugowanie fizyki Chaos. |
| **Cooker Display Mode** | Pokazuje dlaczego asset jest "gotowany" (Instigators). |
| **Insights Task Channel** | Widok zależności zadań w Unreal Insights. |
| **Target Frame Rate** | Skaluj ustawienia (Scalability) pod docelowe FPS, a nie na maxa. |
| **Disable Occluder** | Wyłącz okluzję dla małych/dziurawych obiektów. |
| **dumpticks** | Wypisuje listę wszystkich obiektów wykonujących Tick. |
| **dumpconsolevars** | Zrzuca stan wszystkich zmiennych konsolowych. |
| **RVT Landscape** | Runtime Virtual Texture dla optymalizacji terenu. |
| **Cache Data** | Nie pytaj o dane (np. DataTable) co klatkę – zapisz je. |
| **Runtime Cell Transformer** | Konwersja Static Mesh na Instanced Static Mesh (World Partition). |
| **Bake Water Sim** | Wypalanie symulacji wody dla wydajności. |
| **DisableAllScreenMessages** | Ukrywa komunikaty ekranowe ("Lighting needs to be rebuilt"). |
| **PP Volume vs CVars** | PP Volume nadpisuje CVars (uwaga na interpolację wartości 0-1). |
| **Device Profiles** | Testowanie profili urządzeń w edytorze (`dp.override`). |
| **Actor Coloration** | Wizualizacja aktorów kolorami wg zmiennych. |
| **Debug Float Values** | Wyświetlanie liczb nad obiektami w świecie gry. |
| **Dynamic Mesh Pool** | Pula pamięci dla dynamicznych meshy (unikanie realokacji). |
| **Async Message System** | Komunikacja bez twardych referencji (dobra dla RAM). |
| **Asset Validation** | Własne reguły walidacji (np. nazewnictwo) przy zapisie. |

#### 4. Grafika, Materiały i Animacja
| Skrót / Funkcja | Opis |
| :--- | :--- |
| **Normal Map Packing** | Blue channel jako maska, rekonstrukcja normala z RG. |
| **Bake Vertex Data** | Wypalanie AO/Curvature do Vertex Color (Modeling Mode). |
| **Force Mip Levels** | Wymuś załadowanie tekstury (przydatne przy RenderTarget). |
| **GBuffer in Niagara** | Czytanie koloru/głębi/normali sceny w cząsteczkach. |
| **Volumetric Fog Mat** | Materiał wolumetryczny do lokalnej kontroli mgły. |
| **Negative Desaturate** | Ujemna desaturacja = zwiększenie nasycenia kolorów. |
| **Camera Shake Preview** | Podgląd trzęsienia kamery bezpośrednio w edytorze. |
| **Convex Decomposition** | Automatyczne generowanie precyzyjnej kolizji (Modeling Tools). |
| **Day Sequence Actor** | Prosty system dnia i nocy. |
| **Celestial Vault** | Zaawansowane niebo (gwiazdy, droga mleczna). |
| **Niagara Gameplay** | Używanie Niagary do logiki (ślady stóp, pnącza, fizyka). |
| **Control Rig Direct** | Mapowanie zmiennych BP wprost do Control Rig (bez AnimBP). |
| **CR Secondary Motion** | Proceduralna animacja (Springs, Harmonics) w Control Rig. |
| **CineCamera Tracking** | Wbudowane śledzenie celu (LookAt / Focus). |

#### 5. Różne / Gameplay
| Skrót / Funkcja | Opis |
| :--- | :--- |
| **Editor Only Actor** | Aktorzy, którzy istnieją tylko w edytorze (nie w buildzie). |
| **State Tree** | Ogólna maszyna stanów (nie tylko dla AI). |
| **UEFN** | Prototypowanie multiplayera w edytorze Fortnite. |
| **Promote Metadata** | Dodawanie własnych kolumn/filtrów w Content Browser. |
| **Asset User Data** | Przechowywanie dowolnych danych w assetach. |
| **PCG Shape Grammar** | Gramatyka kształtów do generowania budynków w PCG. |
| **PlayFromHere Check** | Wykrywanie w kodzie, czy gra ruszyła z "Play From Here". |
| **Curve Atlas** | Przechowywanie wielu krzywych w jednej teksturze (dla materiałów). |
| **Flipbooks in Widget** | Używanie animacji Flipbook bezpośrednio w UI (UMG). |
| **Common UI** | Plugin do obsługi UI na wielu platformach (gamepad/mysz). |
| **Smart Objects** | System interakcji AI z otoczeniem (np. ławka do siadania). |
