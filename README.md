# 📉 Analiza wariantowa automatycznych mechanizmów oszczędnościowych (Smart Saver)

### 📈 Podgląd raportu
![Raport Smart Saver]([https://github.com/KamilDataAnalyst/Analiza_wariantowa_automatycznych_mechanizmow_oszczednosciowych_w_aplikacji_bankowej/blob/29c338eb5788915d326c71e4f47da37cdb4bded4/Raport%20pogl%C4%85dowy](https://github.com/KamilDataAnalyst/Analiza_wariantowa_automatycznych_mechanizmow_oszczednosciowych_w_aplikacji_bankowej/blob/5dc4ba1810ea17bf4bc467405e1b666b5992fbed/Pierwszy%20raport%20analityczny.png)
)

---

### 🎯 Cel projektu
Celem raportu była weryfikacja efektywności różnych wariantów automatycznego oszczędzania. Skupiłem się na znalezieniu balansu między maksymalizacją odkładanych kwot a utrzymaniem bezpiecznego salda końcowego, aby uniknąć deficytu budżetowego.

### 💡 Kluczowe wnioski (Data Insights)
* **Ryzyko mechanizmu zaokrągleń:** Wariant "Zaokrąglenie do 5 zł" generuje najwyższe oszczędności przy dużej liczbie transakcji, jednak jest obarczony wysokim ryzykiem. W listopadzie doprowadził do przekroczenia realnej nadwyżki budżetowej, skutkując **ujemnym saldem końcowym (-17,00 zł)**.
* **Optymalny wybór (7%):** Analiza wykazała, że wariant procentowy (7%) jest najbardziej stabilny. Pozwala na zachowanie zrównoważonego salda przy jednoczesnym zachowaniu wysokiej proporcji odkładanych środków względem wydatków.
* **Charakterystyka wydatków:** Listopad, mimo podobnej sumy wydatków co luty, charakteryzował się większą liczbą drobnych transakcji (75% poniżej 10 zł), co drastycznie wpłynęło na efektywność (i ryzyko) mechanizmu zaokrągleń.

### 🛠️ Warsztat techniczny (Excel)
W projekcie wykorzystałem formuły Excela do symulacji różnych scenariuszy na podstawie danych transakcyjnych:
* **Logika warunkowa:** Wykorzystanie funkcji `JEŻELI` (IF) oraz `LUB` (OR) do kategoryzacji transakcji.
* **Matematyka finansowa:** Funkcje zaokrąglające zagnieżdżone w formułach oraz funkcje agregujące (`SUMA`, `ŚREDNIA`).
* **Wizualizacja:** Dynamiczne wykresy relacji między oszczędnościami a saldem dla łatwiejszej interpretacji trendów.
