# Elizaveta Starovoytova
#### (Intern Frontend Developer)
---
### Contact information
__Phone__: 
* +375445474684 (Belarus)
* +79500197909 (Russian Federation)

__E-mail__: lstarovoytova17@gmail.com
__Telegram__: @elizabetast
__Github__: https://github.com/elizabetast
___
### About myself
You can say that my involvement in IT began back in the 9th grade, when I was involved in children's IT school ITeen. Then I took a course in web development, or rather studied HTML/CSS. After graduating from grade 11, I entered the ITMO University, majoring in "Mobile and network technologies". I have already managed to try myself as a designer and project manager on several training projects. At the moment I'm working as a sales manager at the outsourcing agency FedAG, as well as a co-founder of the young company Stellaris Innovations. i

In my free time I like traveling, skiing and reading fiction, psychology. Since childhood, I always know exactly what I want and achieve my goals. I appreciate qualities such as diligence, responsibility, communication skills, ability to negotiate and persistence. Also, I have a trait, which is good in work, but not in real life: fanaticism.

I like the frontend development profession because you can immediately see the result, get a nice picture and experiment. At this stage I have a basic knowledge of HTML/CSS/JS. In life I adhere to the rule ___"You will get exactly as much result as you have worked for"___ , therefore my desire to try and learn, the experience I have gained in life will lead me to my goal to become a good front-end developer.
___
### Skills

__Technical__:
+ HTML/CSS
+ JavaScript (initial level, read code)
+ Python (read code, write code and algorithms)
+ Java (read code)
+ C# (write code, basic level, OOP)
+ MySQL, MongoDB, PostgreSQL
+ Bash (basic)
+ VCS: GitHub, Git
+ IDEs/Soft: PyCharm, Rider, IntelliJ, Webstorm, VS code
+ Design: Figma, Photoshop, Illustrator

__Soft__:
+ Creative
+ Flexible
+ Multitasking
+ Progressive
+ Team-building
+ Sociability

__Language__;
+ Russian/Belarussian (native - C2)
+ English (B2 - exam at ITMO University)
___
### Work experience

April, 2023 - present (Saint-P.)
__Sale/product-manager (FedAG)__
- I deal with the external policy of the outsourcing agency
- I communicate with customers
- Search for tenders and procurements
- I manage social networks and write articles
- Interviewing and looking for developers

May, 2023 - present (Saint-P/online)
__Co-founder/product of the outsourcing agency (Stellaris Innovations)__
- Finding Developers
- Search for orders
- Foreign policy development and cooperation
- Communication with customers
- Internet presence and development of social networks

Feb., 2023 - present (ITMO University)
__Co-founder/designer (Service RANDOMCOFFEE ITMO)__
- design development
- management responsibilities
- work with an advertising company
- Writing the service functions in Python

August, 2021 - May, 2023 (online)
__Tutor in math, physics__
___
### Education 

2021 - present (2025)
__Faculty of Infocommunication Technologies, Mobile and Network Technologies, ITMO UNIVERSITY__

2018-2020 (Gomel)
__Web development course at the ITeen children's programming school, supported by Hi-Tech Park__
+ Diploma of the second degree of the 2nd stage of the national contest "Techno-Intellect
+ 4th place in the team hackathon on chat-bot development supported by the British Embassy

2019 - 2021
__Gomel State Regional Lyceum__
Physics and mathematics profile
___
### Code examples

### C#
***
    public PlayerAbstractExtra FindWinningPlayer(List<PlayerAbstractExtra> players)
    {
        PlayerAbstractExtra winningPlayer = null;
        DeckPlayerRanking highestDeckPlayerRanking = DeckPlayerRanking.None;

        foreach (var player in players)
        {
            DeckPlayerRanking deckPlayerRanking = _winningStrategy.GetDeckPlayerRanking(player.DeckUser);

            if (deckPlayerRanking > highestDeckPlayerRanking)
            {
                highestDeckPlayerRanking = deckPlayerRanking;
                winningPlayer = player;
            }
        }
        return winningPlayer;
    }

### Python
***
    def PolyHash(P, l, p, x):
        res = 0
        for i in reversed(range(l)):
            res = (res * x + ord(P[i])) % p
        return res % p


    def PrecomputeHashes(T, l, k, p, x):
        H = [0] * (l - k + 1)
        S = T[l - k: l]
        H[l - k] = PolyHash(S, k, p, x)
        y = 1
        for i in range(1, k + 1):
            y = (y * x) % p
        for i in range(l - k - 1, -1, -1):
            H[i] = (x * H[i + 1] + ord(T[i]) - y * ord(T[i + k]) + p) % p
        return H

### JavaScript
***

    // обработчик события click для кнопок "назад" и "вперед"
        var _controlClick = function (e) {
          if (e.target.classList.contains('slider__control')) {
            e.preventDefault();
            var direction = e.target.classList.contains('slider__control_right') ? 'right' : 'left';
            _transformItem(direction);
          }
        };

        var _setUpListeners = function () {
          // добавление к кнопкам "назад" и "вперед" обрботчика _controlClick для событя click
          _sliderControls.forEach(function (item) {
            item.addEventListener('click', _controlClick);
          });
        }
