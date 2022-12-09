# bonz-ai

Bakgrund
Ni skapa en webbplats åt det hotellet Bonz.ai som erbjuder en AI-driven eko vistelse. Det första steget var att designa sidan i Figma som ni redan gjort och nu kommer vi till nästa fas som är implementation. Ni ska alltså utgå från er grupps designskiss ni designade i förra kursen (UX / UI grunder) och bygga denna i HTML / CSS men individuellt.

Funktionella krav
Dessa är de sidor som ska finnas med om ni har mer i er skiss får ni göra en avvägning vad ni vill ha med men nedan är kraven.

En landningssida (alltså startsida)
En sida om hotellet och dess faciliteter
En bokningssida för att söka och boka rum (ingen funktionalitet behövs utan fejka en sökning där sökresultaten visas statiskt)
All text kan vara lorem ipsum.

Tekniska krav
Sidan ska vara responsiv (d.v.s den ska funka både i desktop och mobilt läge).
Använda dig av semantisk HTML.
Använda CSS Grid och flexbox.
En CSS-fil ska bara användas.
Bilder
Bilder och logotyp hittar ni här.

Betygskriterier
För att få godkänt ska du:

Ha gjort hemsidan responsiv (d.v.s den ska funka både i desktop och mobilt läge).
Använda dig av semantisk HTML.
Använda CSS Grid och flexbox.
Använda dig av de bifogade bilderna.
Det enbart finns en CSS-fil.
För att få Väl Godkänt ska du:

Allt i godkänt
Använda dig av BEM som namnstandard.
Din CSS ska vara strukturerad och tydligt indelad, gärna så komponentbaserad som möjligt. Fick funderingar fråga!
Inlämning sker via Github och Awesomo. Ladda upp ditt projekt på Github. Gå sedan in på Awesomo och kopiera in länken till ditt repo.

Inlämning senast: 9/11 23:59


// CALENDAR HTML //

        <!-- CHECK IN  -->
        <section class="calendar">
            <article class="calendar__header">
              <h2 class="calendar__heading">CHECK IN</h2>
              <p class="calendar__paragraph">December</p>
            </article>
            <article class="calendar__date">
              <div class="calendar__day">M</div>
              <div class="calendar__day">T</div>
              <div class="calendar__day">W</div>
              <div class="calendar__day">T</div>
              <div class="calendar__day">F</div>
              <div class="calendar__day">S</div>
              <div class="calendar__day">S</div>
              <div class="calendar__number"></div>
              <div class="calendar__number">1</div>
              <div class="calendar__number">2</div>
              <div class="calendar__number">3</div>
              <div class="calendar__number">4</div>
              <div class="calendar__number calendar__number--current">5</div>
              <div class="calendar__number">6</div>
              <div class="calendar__number">7</div>
              <div class="calendar__number">8</div>
              <div class="calendar__number">9</div>
              <div class="calendar__number">10</div>
              <div class="calendar__number">11</div>
              <div class="calendar__number">12</div>
              <div class="calendar__number">13</div>
              <div class="calendar__number">14</div>
              <div class="calendar__number">15</div>
              <div class="calendar__number">16</div>
              <div class="calendar__number">17</div>
              <div class="calendar__number">18</div>
              <div class="calendar__number">19</div>
              <div class="calendar__number">20</div>
              <div class="calendar__number">21</div>
              <div class="calendar__number">22</div>
              <div class="calendar__number">23</div>
              <div class="calendar__number">24</div>
              <div class="calendar__number">25</div>
              <div class="calendar__number">26</div>
              <div class="calendar__number">27</div>
              <div class="calendar__number">28</div>
              <div class="calendar__number">29</div>
              <div class="calendar__number">30</div>
              <div class="calendar__number">31</div>
            </article>
        </section>

          <!-- CHECK OUT  -->

        <section class="calendar">
            <article class="calendar__header">
              <h2 class="calendar__heading">CHECK OUT</h2>
              <p class="calendar__paragraph">December</p>
            </article>
            <article class="calendar__date">
              <div class="calendar__day">M</div>
              <div class="calendar__day">T</div>
              <div class="calendar__day">W</div>
              <div class="calendar__day">T</div>
              <div class="calendar__day">F</div>
              <div class="calendar__day">S</div>
              <div class="calendar__day">S</div>
              <div class="calendar__number"></div>
              <div class="calendar__number">1</div>
              <div class="calendar__number">2</div>
              <div class="calendar__number">3</div>
              <div class="calendar__number">4</div>
              <div class="calendar__number calendar__number--current">5</div>
              <div class="calendar__number">6</div>
              <div class="calendar__number">7</div>
              <div class="calendar__number">8</div>
              <div class="calendar__number">9</div>
              <div class="calendar__number">10</div>
              <div class="calendar__number">11</div>
              <div class="calendar__number">12</div>
              <div class="calendar__number">13</div>
              <div class="calendar__number">14</div>
              <div class="calendar__number">15</div>
              <div class="calendar__number">16</div>
              <div class="calendar__number">17</div>
              <div class="calendar__number">18</div>
              <div class="calendar__number">19</div>
              <div class="calendar__number">20</div>
              <div class="calendar__number">21</div>
              <div class="calendar__number">22</div>
              <div class="calendar__number">23</div>
              <div class="calendar__number">24</div>
              <div class="calendar__number">25</div>
              <div class="calendar__number">26</div>
              <div class="calendar__number">27</div>
              <div class="calendar__number">28</div>
              <div class="calendar__number">29</div>
              <div class="calendar__number">30</div>
              <div class="calendar__number">31</div>
            </article>
          </section>


          // CALENDAR CSS //


/* CALENDAR SECTION  */

header {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1px;
    margin: 2px;
}

.calendar {
    position: relative;
    max-width: 255px;
    background-color: rgb(200, 200, 200);
    box-shadow: 0 5px 50px rgba(#000, 0.5);
    border-radius: 8px;
    overflow: hidden;
  }
  
  .calendar__header {
    position: relative;
    padding: 10px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  
  .calendar__heading {
    margin: 0;
    color: white;
  }
  
  .calendar__paragraph {
    margin: 0;
    font-weight: 500;
  }
  
  .calendar__date {
    padding: 10px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(25px, 1fr));
    grid-gap: 6px;
    box-sizing: border-box;
  }
  
  .calendar__day {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 15px;
    font-weight: 600;
    color: #262626;
  }
  
  .calendar__day:nth-child(7) {
    color: #ff685d;
  }
  
  .calendar__number {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 15px;
    color: #262626;
  }
  
  .calendar__number:nth-child(7n) {
    color: #ff685d;
    font-weight: 700;
  }
  .calendar__number--current,
  .calendar__number:hover {
    background-color: var(--color-booking-button);
    color: #fff !important;
    font-weight: 700;
    cursor: pointer;
    border-radius: 50%;
  }




        <img src="/assets/photos/CHECKIN.jpg" alt="CHECKIN">
        <img src="/assets/photos/CHECKOUT.jpg" alt="CHECKOUT">


.footer__contact, .footer__about, a:link {
    color: black;
    text-decoration: none;
}

.footer__contact span {
    font-weight: 800;
}