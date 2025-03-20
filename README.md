# 📌 Inception tijdlijn

## 📅 Week 1 [24/02/2025 - 02/03/2025]

### 🎯 Doelen

- [x] onderzoek doen naar scrollanimaties
- [x] Elementen die ik erin wil verwerken onder elkaar zetten

### ✅ To-Do Lijst

- [x] Inception kijken
- [x] Elementen zoeken
- [x] basisopzet coderen html

### 📝 Vorderingen & Notities]

- **Opdracht:**

Een van mijn doelen is natuurlijk om scrollanimaties onder de knie te krijgen. De film tijdlijn opdracht is een goede kans op daar aan te kunnen werken. Inception had ik nog niet eerder gezien, maar kende de hoofdlijn van de film wel. In inception gaan ze een droom in een droom in een droom in. Hoe ik dit wil gaan laten zien in een website weet ik nog niet. Maar ik denk dat ik met scrollanimaties wel ver kom.

- **Wat heb ik deze week gedaan?:**

- de film gekeken en besloten welke elementen ik wil gaan uitwerken om mijn skills in css te verbeteren.

  1. De totems die worden gebruikt om na te gaan of het realiteit of een droom is bouwen
  2. de manier waarop ze uit de dromen komen -> doormiddel van een schok/bijna dood gaan, of een val
  3. Typografie: Rood, vervorming, groot en bold.
  4. De bron hieronder kan ik gebruiken om misschien een soort basis te bouwen of erachter te komen hoe scroll animaties werken.

- **Bronnen**
  https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_scroll-driven_animations

---

## 📅 Week 2 [03/03/2025 - 09/03/2025]

### 🎯 Doelen

- [ ] Hoe ga ik droom in droom visualiseren?
- [x] Dobbelsteen maken
- [x] Heading scroll animatie

### ✅ To-Do Lijst

- [x] Tol svg maken
- [x] Dobbelsteen maken
- [x] Dobbelsteen animeren
- [x] Dobbelsteen animeren op scroll event
- [x] Gradients dobbelsteen fixen
- [ ] Horizontale scroll section -> reality

### 📝 Obstakels & Notities

- **Vorderingen:**

Ik wil (ondanks dat ik weet dat het qua UX niet top is) de horizontale scroll section onder de knie krijgen. Dit is iets wat ik veel voorbij heb zien komen in veel websites. Daarnaast vind ik het een film achtig idee geven (alsof je een tape doorkijkt). En ondanks dat dit misschien niet een eigen experiment was, maar meer onderzoek en nadoen, heb ik er wel veel van geleerd. Zie stuk code:

``css

@keyframes move {
to {
/_ Move horizontally so that right edge is aligned against the viewport _/
transform: translateX(calc(-100% + 100vw));
}
}

div:nth-of-type(2) section:nth-of-type(1) {
background-color: rgb(19, 18, 18);
height: 500vh;
overflow: visible; /_ To make position sticky work … _/

    view-timeline-name: --section-pin-tl;
    view-timeline-axis: block;


    & div {
        /* Stick to Top */
        height: 110vh;
        width: 100vw;
        position: sticky;
        top: 0;
        padding: 0;
        margin: 0;

        width: 100vw;
        overflow-x: hidden;


        & ul {
            display: flex;
            list-style: none;
            align-items: center;
            gap: 150px;
            height: 100vh;
            width: 230vmax;

            /* Hook animation */
            will-change: transform;
            animation: linear move forwards;

            /* Link animation to view-timeline */
            animation-timeline: --section-pin-tl;
            animation-range: contain 0% contain 100%;

            & li {
                text-align: left;
                max-width: 700px;
                padding: 100px;
                color: white;

                & h3 {
                    font-family: "scale-variable", sans-serif;
                    font-variation-settings: "wght" 300, "wdth" 100;
                    font-size: 4em;
                }

                & p {
                    width: 100%;
                    font-family: "scandia-web", sans-serif;
                    font-weight: 400;
                    font-style: normal;
                    font-size: 1.1em;
                    line-height: 25px;
                }
            }
        }
    }

}

``

Deze week heb ik mijn dobbelsteen gemaakt en verbeterd. Ik had gradients gemaakt die de stippen moesten voorstellen maar dat gedaan doormiddel van procenten, niet em/px. Hierdoor waren de stippen niet gelijk. Dit heb ik opgelost! Daarnaast animeert hij nu wel op scroll, terwijl het eerst infinite was.

- **Problemen**

Ik kan nogsteeds niet bedenken hoe ik een droom in droom moet gaan vertonen.

-**Bronnen:**

https://scroll-driven-animations.style/

Horizontal scroll

https://scroll-driven-animations.style/demos/horizontal-section/css/

---

## 📅 Week 3 [10/03/2025 - 16/03/2025]

### 🎯 Doelen

- [ ] Droom in droom visualiseren

### ✅ To-Do Lijst

- [ ] Content in de dreams

### 📝 Obstakels & Notities

- **Probleem:**

Ik merk dat ik moeite heb met het bedenken en visualiseren in mijn hoofd wat voor animaties ik kan toepassen. Mijn creativiteit stopt daar een beetje. Omdat ik in mijn hoofd veel chaos beleef vind ik het nog moeilijk om animaties in stappen uit te werken. Ik probeer daarom inspiratie op te doen bij andere mensen, maar merk dan snel dat ik dingen overneem en vervolgens niet meer aanpas, waardoor het hele experimenteren van dit vak moeilijk gaat.

Ik liep deze week heel erg vast met het coderen van een droom in een droom etc. Ik begon met experimenteren, met een codepen van Sanne (zie bronvermelding), maar kwam na een hele dag eraan werken nergens. Ik was te chaotisch in de dingen die ik moest toevoegen verwijderen en merkte dat ik gewoon niet opschoot. Toen verloor ik een beetje mijn hoop en ben ik teruggegaan naar de Mozilla bron waar ik de scrollbased stacking cards van heb gebruikt. Mijn plan is om die code als basis een beetje te gebruiken / bouwen op mijn eigen manier, en op zon manier de animaties uitwerken dat elke foto steeds kleiner wordt en dieper in elkaar gaat. Op die manier zou ik dan een droom in een droom weergeven.
Verder zou ik dus iets willen doen met hue veranderingen, trillingen en vervaging om dan een droom te realiseren.

![stackingcards](./images/Screenshot%202025-03-20%20at%2015.23.06.png)

(week 4 ik: Helaas heb ik er geen screenshot van gemaakt dus kan het niet laten zien. Wel zet ik de bron erin die ik heb gebruikt. Uiteindelijk is het niet in het eindproduct gekomen dus of het veel uit maakt weet ik.)

---

## 📅 Week 4 [10/03/2025 - 16/03/2025]

### 🎯 Doelen

- [ ] Responsive
- [ ] Droom in een droom in een droom visualiseren

### ✅ To-Do Lijst

- [ ] header color difference ding (naam vergeten)
- [ ] Content in de dreams

### 📝 Obstakels & Notities

- **Probleem:**
- **Oplossing:**
