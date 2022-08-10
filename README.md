# Markdown

## Markdown

### Headings

**Rendered**

## Heading 1 {docsify-ignore}

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse luctus nulla eu ex varius, a varius elit tincidunt. Aenean arcu magna, gravida id purus a, interdum convallis turpis. Aenean id ipsum eu tortor sollicitudin scelerisque in quis elit.

### Heading 2 {docsify-ignore}

Vestibulum lobortis laoreet nunc vel vulputate. In et augue non lectus pellentesque molestie et ac justo. Sed sed turpis ut diam gravida sagittis nec at neque. Vivamus id tellus est. Nam ac dignissim mi. Vestibulum nec sem convallis, condimentum augue at, commodo diam.

#### Heading 3 {docsify-ignore}

Suspendisse sit amet tincidunt nibh, ac interdum velit. Ut orci diam, dignissim at enim sit amet, placerat rutrum magna. Mauris consectetur nibh eget sem feugiat, sit amet congue quam laoreet. Curabitur sed massa metus.

**Heading 4 {docsify-ignore}**

Donec odio orci, facilisis ac vehicula in, vestibulum ut urna. Ut bibendum ullamcorper risus, ac euismod leo maximus sed. In pulvinar sagittis rutrum. Morbi quis cursus diam. Cras ac laoreet nulla, rhoncus sodales dui.

**Heading 5 {docsify-ignore}**

Commodo sit veniam nulla cillum labore ullamco aliquip quis. Consequat nulla fugiat consequat ex duis proident. Adipisicing excepteur tempor exercitation ad. Consectetur voluptate Lorem sint elit exercitation ullamco dolor.

**Heading 6 {docsify-ignore}**

Ipsum ea amet dolore mollit incididunt fugiat nulla laboris est sint voluptate. Ex culpa id amet ipsum amet pariatur ipsum officia sit laborum irure ullamco deserunt. Consequat qui tempor occaecat nostrud proident.

**Markdown**

```markdown
# Heading 1

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse luctus
nulla eu ex varius, a varius elit tincidunt. Aenean arcu magna, gravida id purus
a, interdum convallis turpis. Aenean id ipsum eu tortor sollicitudin scelerisque
in quis elit.

## Heading 2

Vestibulum lobortis laoreet nunc vel vulputate. In et augue non lectus
pellentesque molestie et ac justo. Sed sed turpis ut diam gravida sagittis nec
at neque. Vivamus id tellus est. Nam ac dignissim mi. Vestibulum nec sem
convallis, condimentum augue at, commodo diam.

### Heading 3

Suspendisse sit amet tincidunt nibh, ac interdum velit. Ut orci diam, dignissim
at enim sit amet, placerat rutrum magna. Mauris consectetur nibh eget sem
feugiat, sit amet congue quam laoreet. Curabitur sed massa metus.

#### Heading 4

Donec odio orci, facilisis ac vehicula in, vestibulum ut urna. Ut bibendum
ullamcorper risus, ac euismod leo maximus sed. In pulvinar sagittis rutrum.
Morbi quis cursus diam. Cras ac laoreet nulla, rhoncus sodales dui.

##### Heading 5

Commodo sit veniam nulla cillum labore ullamco aliquip quis. Consequat nulla
fugiat consequat ex duis proident. Adipisicing excepteur tempor exercitation ad.
Consectetur voluptate Lorem sint elit exercitation ullamco dolor.

###### Heading 6

Ipsum ea amet dolore mollit incididunt fugiat nulla laboris est sint voluptate.
Ex culpa id amet ipsum amet pariatur ipsum officia sit laborum irure ullamco
deserunt. Consequat qui tempor occaecat nostrud proident.
```

### Text

**Rendered**

Body text

**Bold text**

_Italic text_

~~Strikethrough~~

Marked text

```
Preformatted text
```

Small Text

This is subscript

This is superscript

**Markdown**

```markdown
Body text

**Bold text**

*Italic text*

~~Strikethrough~~

<mark>Marked text</mark>

<pre>Preformatted text</pre>

<small>Small Text</small>

This is <sub>subscript</sub>

This is <sup>superscript</sup>
```

### Links

**Rendered**

[Inline link](https://google.com)

[Inline link with title](https://google.com)

[Reference link by name](https://google.com)

[Reference link by number](https://google.com)

[Reference link by self](https://google.com)

**Markdown**

```markdown
[Inline link](https://google.com)

[Inline link with title](https://google.com "Google")

[Reference link by name][link1]

[Reference link by number][1]

[Reference link by self]

[link1]: https://google.com
[1]: https://google.com
[Reference link by self]: https://google.com
```

### Lists

**Rendered**

**Ordered Lists**

1. Ordered 1
2. Ordered 2
   1. Ordered 2a
   2. Ordered 2b
   3. Ordered 2c
3. Ordered 3

**Unordered Lists**

* Unordered 1
* Unordered 2
  * Unordered 2a
  * Unordered 2b
  * Unordered 2c
* Unordered 3

**Task Lists**

* [x] Task 1
* [ ] Task 2
  * [x] Subtask A
  * [ ] Subtask B
* [ ] Task 3

**Markdown**

```markdown
**Ordered Lists**

1. Ordered 1
1. Ordered 2
   1. Ordered 2a
   1. Ordered 2b
   1. Ordered 2c
1. Ordered 3

**Unordered Lists**

- Unordered 1
- Unordered 2
  - Unordered 2a
  - Unordered 2b
  - Unordered 2c
- Unordered 3

**Task Lists**

- [x] Task 1
- [ ] Task 2
  - [x] Subtask A
  - [ ] Subtask B
- [ ] Task 3
```

### Blockquotes

**Rendered**

> Cras aliquet nulla quis metus tincidunt, sed placerat enim cursus. Etiam turpis nisl, posuere eu condimentum ut, interdum a risus. Sed non luctus mi. Quisque malesuada risus sit amet tortor aliquet, a posuere ex iaculis. Vivamus ultrices enim dui, eleifend porttitor elit aliquet sed.
>
> _- Quote Source_

**Markdown**

```markdown
> Cras aliquet nulla quis metus tincidunt, sed placerat enim cursus. Etiam
> turpis nisl, posuere eu condimentum ut, interdum a risus. Sed non luctus mi.
> Quisque malesuada risus sit amet tortor aliquet, a posuere ex iaculis. Vivamus
> ultrices enim dui, eleifend porttitor elit aliquet sed.
>
> *- Quote Source*
```

### Code

**Rendered**

This is `inline code`

```javascript
const add   = (num1, num2) => num1 + num2;
const total = add(1, 2);

console.log(total); // 3
```

```html
<body>
    <p>Hello</p>
</body>
```

**Markdown**

````markdown
This is `inline code`

```javascript
const add   = (num1, num2) => num1 + num2;
const total = add(1, 2);

console.log(total); // 3
```

```html
<body>
    <p>Hello</p>
</body>
```
````

### Notices

**Rendered**

!> **Important** notice with `inline code` and additional placeholder text used to force the content to wrap and span multiple lines.

?> **Tip** notice with `inline code` and additional placeholder text used to force the content to wrap and span multiple lines.

**Markdown**

```markdown
!> **Important** notice with `inline code` and additional placeholder text used
to force the content to wrap and span multiple lines.

?> **Tip** notice with `inline code` and additional placeholder text used to
force the content to wrap and span multiple lines.
```

### Tabs

Tabs provided via the [docsify-tabs](https://jhildenbiddle.github.io/docsify-tabs) plugin.

**English**

Hello!

**French**

Bonjour!

**Italian**

Ciao!

**Markdown**

```markdown
<!-- tabs:start -->

#### **English**

Hello!

#### **French**

Bonjour!

#### **Italian**

Ciao!

<!-- tabs:end -->
```

### Tables

**Rendered**

| Left Align | Center Align | Right Align | Non‑Breaking Header |
| ---------- | :----------: | ----------: | ------------------- |
| A1         |      A2      |          A3 | A4                  |
| B1         |      B2      |          B3 | B4                  |
| C1         |      C2      |          C3 | C4                  |

**Markdown**

```markdown
| Left Align | Center Align | Right Align | Non&#8209;Breaking&nbsp;Header |
| ---------- |:------------:| -----------:| ------------------------------ |
| A1         | A2           | A3          | A4                             |
| B1         | B2           | B3          | B4                             |
| C1         | C2           | C3          | C4                             |
```

### Keyboard

**Rendered**

↑ Arrow Up

↓ Arrow Down

← Arrow Left

→ Arrow Right

⇪ Caps Lock

⌘ Command

⌃ Control

⌫ Delete

⌦ Delete (Forward)

↘ End

⌤ Enter

⎋ Escape

↖ Home

⇞ Page Up

⇟ Page Down

⌥ Option, Alt

↵ Return

⇧ Shift

␣ Space

⇥ Tab

⇤ Tab + Shift

**Markdown**

```markdown
<kbd>&uarr;</kbd> Arrow Up

<kbd>&darr;</kbd> Arrow Down

<kbd>&larr;</kbd> Arrow Left

<kbd>&rarr;</kbd> Arrow Right

<kbd>&#8682;</kbd> Caps Lock

<kbd>&#8984;</kbd> Command

<kbd>&#8963;</kbd> Control

<kbd>&#9003;</kbd> Delete

<kbd>&#8998;</kbd> Delete (Forward)

<kbd>&#8600;</kbd> End

<kbd>&#8996;</kbd> Enter

<kbd>&#9099;</kbd> Escape

<kbd>&#8598;</kbd> Home

<kbd>&#8670;</kbd> Page Up

<kbd>&#8671;</kbd> Page Down

<kbd>&#8997;</kbd> Option, Alt

<kbd>&#8629;</kbd> Return

<kbd>&#8679;</kbd> Shift

<kbd>&#9251;</kbd> Space

<kbd>&#8677;</kbd> Tab

<kbd>&#8676;</kbd> Tab + Shift
```

### Horizontal Rule

**Rendered**

***

**Markdown**

```markdown
---
```

### Images

**Rendered**

Inline-style

![alt text](https://source.unsplash.com/daily)

Reference-style

![alt text](https://source.unsplash.com/collection/881815)

**Markdown**

```markdown
**Inline**

![alt text](//source.unsplash.com/daily "Provided by unsplash.com")

**Reference**

![alt text][logo]

[logo]: //source.unsplash.com/collection/881815 "Provided by unsplash.com"
```

### Emoji

A complete list is available here: [Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet/)

**Rendered**

**People**

:bowtie: :smile: :laughing: :blush: :smiley: :relaxed: :smirk: :heart\_eyes: :kissing\_heart: :kissing\_closed\_eyes: :flushed: :relieved: :satisfied: :grin: :wink: :stuck\_out\_tongue\_winking\_eye: :stuck\_out\_tongue\_closed\_eyes: :grinning: :kissing: :kissing\_smiling\_eyes: :stuck\_out\_tongue: :sleeping: :worried: :frowning: :anguished: :open\_mouth: :grimacing: :confused: :hushed: :expressionless: :unamused: :sweat\_smile: :sweat: :disappointed\_relieved: :weary: :pensive: :disappointed: :confounded: :fearful: :cold\_sweat: :persevere: :cry: :sob: :joy: :astonished: :scream: :neckbeard: :tired\_face: :angry: :rage: :triumph: :sleepy: :yum: :mask: :sunglasses: :dizzy\_face: :imp: :smiling\_imp: :neutral\_face: :no\_mouth: :innocent: :alien: :yellow\_heart: :blue\_heart: :purple\_heart: :heart: :green\_heart: :broken\_heart: :heartbeat: :heartpulse: :two\_hearts: :revolving\_hearts: :cupid: :sparkling\_heart: :sparkles: :star: :star2: :dizzy: :boom: :collision: :anger: :exclamation: :question: :grey\_exclamation: :grey\_question: :zzz: :dash: :sweat\_drops: :notes: :musical\_note: :fire: :hankey: :poop: :shit: :thumbsup: :thumbsdown: :ok\_hand: :punch: :facepunch: :fist: :v: :wave: :hand: :raised\_hand: :open\_hands: :point\_up: :point\_down: :point\_left: :point\_right: :raised\_hands: :pray: :point\_up\_2: :clap: :muscle: :metal: :fu: :runner: :running: :couple: :family: :two\_men\_holding\_hands: :two\_women\_holding\_hands: :dancer: :dancers: :ok\_woman: :no\_good: :information\_desk\_person: :raising\_hand: :bride\_with\_veil: :person\_with\_pouting\_face: :person\_frowning: :bow: :couplekiss: :couple\_with\_heart: :massage: :haircut: :nail\_care: :boy: :girl: :woman: :man: :baby: :older\_woman: :older\_man: :person\_with\_blond\_hair: :man\_with\_gua\_pi\_mao: :man\_with\_turban: :construction\_worker: :cop: :angel: :princess: :smiley\_cat: :smile\_cat: :heart\_eyes\_cat: :kissing\_cat: :smirk\_cat: :scream\_cat: :crying\_cat\_face: :joy\_cat: :pouting\_cat: :japanese\_ogre: :japanese\_goblin: :see\_no\_evil: :hear\_no\_evil: :speak\_no\_evil: :guardsman: :skull: :feet: :lips: :kiss: :droplet: :ear: :eyes: :nose: :tongue: :love\_letter: :bust\_in\_silhouette: :busts\_in\_silhouette: :speech\_balloon: :thought\_balloon: :feelsgood: :finnadie: :goberserk: :godmode: :hurtrealbad: :rage1: :rage2: :rage3: :rage4: :suspect: :trollface:

**Nature**

:sunny: :umbrella: :cloud: :snowflake: :snowman: :zap: :cyclone: :foggy: :ocean: :cat: :dog: :mouse: :hamster: :rabbit: :wolf: :frog: :tiger: :koala: :bear: :pig: :pig\_nose: :cow: :boar: :monkey\_face: :monkey: :horse: :racehorse: :camel: :sheep: :elephant: :panda\_face: :snake: :bird: :baby\_chick: :hatched\_chick: :hatching\_chick: :chicken: :penguin: :turtle: :bug: :honeybee: :ant: :beetle: :snail: :octopus: :tropical\_fish: :fish: :whale: :whale2: :dolphin: :cow2: :ram: :rat: :water\_buffalo: :tiger2: :rabbit2: :dragon: :goat: :rooster: :dog2: :pig2: :mouse2: :ox: :dragon\_face: :blowfish: :crocodile: :dromedary\_camel: :leopard: :cat2: :poodle: :paw\_prints: :bouquet: :cherry\_blossom: :tulip: :four\_leaf\_clover: :rose: :sunflower: :hibiscus: :maple\_leaf: :leaves: :fallen\_leaf: :herb: :mushroom: :cactus: :palm\_tree: :evergreen\_tree: :deciduous\_tree: :chestnut: :seedling: :blossom: :ear\_of\_rice: :shell: :globe\_with\_meridians: :sun\_with\_face: :full\_moon\_with\_face: :new\_moon\_with\_face: :new\_moon: :waxing\_crescent\_moon: :first\_quarter\_moon: :waxing\_gibbous\_moon: :full\_moon: :waning\_gibbous\_moon: :last\_quarter\_moon: :waning\_crescent\_moon: :last\_quarter\_moon\_with\_face: :first\_quarter\_moon\_with\_face: :crescent\_moon: :earth\_africa: :earth\_americas: :earth\_asia: :volcano: :milky\_way: :partly\_sunny: :octocat: :squirrel:

**Objects**

:bamboo: :gift\_heart: :dolls: :school\_satchel: :mortar\_board: :flags: :fireworks: :sparkler: :wind\_chime: :rice\_scene: :jack\_o\_lantern: :ghost: :santa: :christmas\_tree: :gift: :bell: :no\_bell: :tanabata\_tree: :tada: :confetti\_ball: :balloon: :crystal\_ball: :cd: :dvd: :floppy\_disk: :camera: :video\_camera: :movie\_camera: :computer: :tv: :iphone: :phone: :telephone: :telephone\_receiver: :pager: :fax: :minidisc: :vhs: :sound: :speaker: :mute: :loudspeaker: :mega: :hourglass: :hourglass\_flowing\_sand: :alarm\_clock: :watch: :radio: :satellite: :loop: :mag: :mag\_right: :unlock: :lock: :lock\_with\_ink\_pen: :closed\_lock\_with\_key: :key: :bulb: :flashlight: :high\_brightness: :low\_brightness: :electric\_plug: :battery: :calling: :email: :mailbox: :postbox: :bath: :bathtub: :shower: :toilet: :wrench: :nut\_and\_bolt: :hammer: :seat: :moneybag: :yen: :dollar: :pound: :euro: :credit\_card: :money\_with\_wings: :inbox\_tray: :outbox\_tray: :envelope: :incoming\_envelope: :postal\_horn: :mailbox\_closed: :mailbox\_with\_mail: :mailbox\_with\_no\_mail: :package: :door: :smoking: :bomb: :gun: :hocho: :pill: :syringe: :page\_facing\_up: :page\_with\_curl: :bookmark\_tabs: :bar\_chart: :chart\_with\_upwards\_trend: :chart\_with\_downwards\_trend: :scroll: :clipboard: :calendar: :date: :card\_index: :file\_folder: :open\_file\_folder: :scissors: :pushpin: :paperclip: :black\_nib: :pencil2: :straight\_ruler: :triangular\_ruler: :closed\_book: :green\_book: :blue\_book: :orange\_book: :notebook: :notebook\_with\_decorative\_cover: :ledger: :books: :bookmark: :name\_badge: :microscope: :telescope: :newspaper: :football: :basketball: :soccer: :baseball: :tennis: :8ball: :rugby\_football: :bowling: :golf: :mountain\_bicyclist: :bicyclist: :horse\_racing: :snowboarder: :swimmer: :surfer: :ski: :spades: :hearts: :clubs: :diamonds: :gem: :ring: :trophy: :musical\_score: :musical\_keyboard: :violin: :space\_invader: :video\_game: :black\_joker: :flower\_playing\_cards: :game\_die: :dart: :mahjong: :clapper: :memo: :pencil: :book: :art: :microphone: :headphones: :trumpet: :saxophone: :guitar: :shoe: :sandal: :high\_heel: :lipstick: :boot: :shirt: :tshirt: :necktie: :womans\_clothes: :dress: :running\_shirt\_with\_sash: :jeans: :kimono: :bikini: :ribbon: :tophat: :crown: :womans\_hat: :mans\_shoe: :closed\_umbrella: :briefcase: :handbag: :pouch: :purse: :eyeglasses: :fishing\_pole\_and\_fish: :coffee: :tea: :sake: :baby\_bottle: :beer: :beers: :cocktail: :tropical\_drink: :wine\_glass: :fork\_and\_knife: :pizza: :hamburger: :fries: :poultry\_leg: :meat\_on\_bone: :spaghetti: :curry: :fried\_shrimp: :bento: :sushi: :fish\_cake: :rice\_ball: :rice\_cracker: :rice: :ramen: :stew: :oden: :dango: :egg: :bread: :doughnut: :custard: :icecream: :ice\_cream: :shaved\_ice: :birthday: :cake: :cookie: :chocolate\_bar: :candy: :lollipop: :honey\_pot: :apple: :green\_apple: :tangerine: :lemon: :cherries: :grapes: :watermelon: :strawberry: :peach: :melon: :banana: :pear: :pineapple: :sweet\_potato: :eggplant: :tomato: :corn:

**Places**

:house: :house\_with\_garden: :school: :office: :post\_office: :hospital: :bank: :convenience\_store: :love\_hotel: :hotel: :wedding: :church: :department\_store: :european\_post\_office: :city\_sunrise: :city\_sunset: :japanese\_castle: :european\_castle: :tent: :factory: :tokyo\_tower: :japan: :mount\_fuji: :sunrise\_over\_mountains: :sunrise: :stars: :statue\_of\_liberty: :bridge\_at\_night: :carousel\_horse: :rainbow: :ferris\_wheel: :fountain: :roller\_coaster: :ship: :speedboat: :boat: :sailboat: :rowboat: :anchor: :rocket: :airplane: :helicopter: :steam\_locomotive: :tram: :mountain\_railway: :bike: :aerial\_tramway: :suspension\_railway: :mountain\_cableway: :tractor: :blue\_car: :oncoming\_automobile: :car: :red\_car: :taxi: :oncoming\_taxi: :articulated\_lorry: :bus: :oncoming\_bus: :rotating\_light: :police\_car: :oncoming\_police\_car: :fire\_engine: :ambulance: :minibus: :truck: :train: :station: :train2: :bullettrain\_front: :bullettrain\_side: :light\_rail: :monorail: :railway\_car: :trolleybus: :ticket: :fuelpump: :vertical\_traffic\_light: :traffic\_light: :warning: :construction: :beginner: :atm: :slot\_machine: :busstop: :barber: :hotsprings: :checkered\_flag: :crossed\_flags: :izakaya\_lantern: :moyai: :circus\_tent: :performing\_arts: :round\_pushpin: :triangular\_flag\_on\_post: :jp: :kr: :cn: :us: :fr: :es: :it: :ru: :gb: :uk: :de:

**Symbols**

:one: :two: :three: :four: :five: :six: :seven: :eight: :nine: :keycap\_ten: :1234: :zero: :hash: :symbols: :arrow\_backward: :arrow\_down: :arrow\_forward: :arrow\_left: :capital\_abcd: :abcd: :abc: :arrow\_lower\_left: :arrow\_lower\_right: :arrow\_right: :arrow\_up: :arrow\_upper\_left: :arrow\_upper\_right: :arrow\_double\_down: :arrow\_double\_up: :arrow\_down\_small: :arrow\_heading\_down: :arrow\_heading\_up: :leftwards\_arrow\_with\_hook: :arrow\_right\_hook: :left\_right\_arrow: :arrow\_up\_down: :arrow\_up\_small: :arrows\_clockwise: :arrows\_counterclockwise: :rewind: :fast\_forward: :information\_source: :ok: :twisted\_rightwards\_arrows: :repeat: :repeat\_one: :new: :top: :up: :cool: :free: :ng: :cinema: :koko: :signal\_strength: :u5272: :u5408: :u55b6: :u6307: :u6708: :u6709: :u6e80: :u7121: :u7533: :u7a7a: :u7981: :sa: :restroom: :mens: :womens: :baby\_symbol: :no\_smoking: :parking: :wheelchair: :metro: :baggage\_claim: :accept: :wc: :potable\_water: :put\_litter\_in\_its\_place: :secret: :congratulations: :m: :passport\_control: :left\_luggage: :customs: :ideograph\_advantage: :cl: :sos: :id: :no\_entry\_sign: :underage: :no\_mobile\_phones: :do\_not\_litter: :no\_bicycles: :no\_pedestrians: :children\_crossing: :no\_entry: :eight\_spoked\_asterisk: :sparkle: :eight\_pointed\_black\_star: :heart\_decoration: :vs: :vibration\_mode: :mobile\_phone\_off: :chart: :currency\_exchange: :aries: :taurus: :gemini: :cancer: :leo: :virgo: :libra: :scorpius: :sagittarius: :capricorn: :aquarius: :pisces: :ophiuchus: :six\_pointed\_star: :negative\_squared\_cross\_mark: :a: :b: :ab: :o2: :diamond\_shape\_with\_a\_dot\_inside: :recycle: :end: :back: :on: :soon: :clock1: :clock130: :clock10: :clock1030: :clock11: :clock1130: :clock12: :clock1230: :clock2: :clock230: :clock3: :clock330: :clock4: :clock430: :clock5: :clock530: :clock6: :clock630: :clock7: :clock730: :clock8: :clock830: :clock9: :clock930: :heavy\_dollar\_sign: :copyright: :registered: :tm: :x: :heavy\_exclamation\_mark: :bangbang: :interrobang: :o: :heavy\_multiplication\_x: :heavy\_plus\_sign: :heavy\_minus\_sign: :heavy\_division\_sign: :white\_flower: :100: :heavy\_check\_mark: :ballot\_box\_with\_check: :radio\_button: :link: :curly\_loop: :wavy\_dash: :part\_alternation\_mark: :trident: :black\_small\_square: :white\_small\_square: :black\_medium\_small\_square: :white\_medium\_small\_square: :black\_medium\_square: :white\_medium\_square: :black\_large\_square: :white\_large\_square: :white\_check\_mark: :black\_square\_button: :white\_square\_button: :black\_circle: :white\_circle: :red\_circle: :large\_blue\_circle: :large\_blue\_diamond: :large\_orange\_diamond: :small\_blue\_diamond: :small\_orange\_diamond: :small\_red\_triangle: :small\_red\_triangle\_down: :shipit:

**Markdown**

```markdown
**People**

:bowtie:
:smile:
:laughing:
:blush:
:smiley:
:relaxed:
:smirk:
:heart_eyes:
:kissing_heart:
:kissing_closed_eyes:
:flushed:
:relieved:
:satisfied:
:grin:
:wink:
:stuck_out_tongue_winking_eye:
:stuck_out_tongue_closed_eyes:
:grinning:
:kissing:
:kissing_smiling_eyes:
:stuck_out_tongue:
:sleeping:
:worried:
:frowning:
:anguished:
:open_mouth:
:grimacing:
:confused:
:hushed:
:expressionless:
:unamused:
:sweat_smile:
:sweat:
:disappointed_relieved:
:weary:
:pensive:
:disappointed:
:confounded:
:fearful:
:cold_sweat:
:persevere:
:cry:
:sob:
:joy:
:astonished:
:scream:
:neckbeard:
:tired_face:
:angry:
:rage:
:triumph:
:sleepy:
:yum:
:mask:
:sunglasses:
:dizzy_face:
:imp:
:smiling_imp:
:neutral_face:
:no_mouth:
:innocent:
:alien:
:yellow_heart:
:blue_heart:
:purple_heart:
:heart:
:green_heart:
:broken_heart:
:heartbeat:
:heartpulse:
:two_hearts:
:revolving_hearts:
:cupid:
:sparkling_heart:
:sparkles:
:star:
:star2:
:dizzy:
:boom:
:collision:
:anger:
:exclamation:
:question:
:grey_exclamation:
:grey_question:
:zzz:
:dash:
:sweat_drops:
:notes:
:musical_note:
:fire:
:hankey:
:poop:
:shit:
:thumbsup:
:thumbsdown:
:ok_hand:
:punch:
:facepunch:
:fist:
:v:
:wave:
:hand:
:raised_hand:
:open_hands:
:point_up:
:point_down:
:point_left:
:point_right:
:raised_hands:
:pray:
:point_up_2:
:clap:
:muscle:
:metal:
:fu:
:runner:
:running:
:couple:
:family:
:two_men_holding_hands:
:two_women_holding_hands:
:dancer:
:dancers:
:ok_woman:
:no_good:
:information_desk_person:
:raising_hand:
:bride_with_veil:
:person_with_pouting_face:
:person_frowning:
:bow:
:couplekiss:
:couple_with_heart:
:massage:
:haircut:
:nail_care:
:boy:
:girl:
:woman:
:man:
:baby:
:older_woman:
:older_man:
:person_with_blond_hair:
:man_with_gua_pi_mao:
:man_with_turban:
:construction_worker:
:cop:
:angel:
:princess:
:smiley_cat:
:smile_cat:
:heart_eyes_cat:
:kissing_cat:
:smirk_cat:
:scream_cat:
:crying_cat_face:
:joy_cat:
:pouting_cat:
:japanese_ogre:
:japanese_goblin:
:see_no_evil:
:hear_no_evil:
:speak_no_evil:
:guardsman:
:skull:
:feet:
:lips:
:kiss:
:droplet:
:ear:
:eyes:
:nose:
:tongue:
:love_letter:
:bust_in_silhouette:
:busts_in_silhouette:
:speech_balloon:
:thought_balloon:
:feelsgood:
:finnadie:
:goberserk:
:godmode:
:hurtrealbad:
:rage1:
:rage2:
:rage3:
:rage4:
:suspect:
:trollface:

**Nature**

:sunny:
:umbrella:
:cloud:
:snowflake:
:snowman:
:zap:
:cyclone:
:foggy:
:ocean:
:cat:
:dog:
:mouse:
:hamster:
:rabbit:
:wolf:
:frog:
:tiger:
:koala:
:bear:
:pig:
:pig_nose:
:cow:
:boar:
:monkey_face:
:monkey:
:horse:
:racehorse:
:camel:
:sheep:
:elephant:
:panda_face:
:snake:
:bird:
:baby_chick:
:hatched_chick:
:hatching_chick:
:chicken:
:penguin:
:turtle:
:bug:
:honeybee:
:ant:
:beetle:
:snail:
:octopus:
:tropical_fish:
:fish:
:whale:
:whale2:
:dolphin:
:cow2:
:ram:
:rat:
:water_buffalo:
:tiger2:
:rabbit2:
:dragon:
:goat:
:rooster:
:dog2:
:pig2:
:mouse2:
:ox:
:dragon_face:
:blowfish:
:crocodile:
:dromedary_camel:
:leopard:
:cat2:
:poodle:
:paw_prints:
:bouquet:
:cherry_blossom:
:tulip:
:four_leaf_clover:
:rose:
:sunflower:
:hibiscus:
:maple_leaf:
:leaves:
:fallen_leaf:
:herb:
:mushroom:
:cactus:
:palm_tree:
:evergreen_tree:
:deciduous_tree:
:chestnut:
:seedling:
:blossom:
:ear_of_rice:
:shell:
:globe_with_meridians:
:sun_with_face:
:full_moon_with_face:
:new_moon_with_face:
:new_moon:
:waxing_crescent_moon:
:first_quarter_moon:
:waxing_gibbous_moon:
:full_moon:
:waning_gibbous_moon:
:last_quarter_moon:
:waning_crescent_moon:
:last_quarter_moon_with_face:
:first_quarter_moon_with_face:
:crescent_moon:
:earth_africa:
:earth_americas:
:earth_asia:
:volcano:
:milky_way:
:partly_sunny:
:octocat:
:squirrel:

**Objects**

:bamboo:
:gift_heart:
:dolls:
:school_satchel:
:mortar_board:
:flags:
:fireworks:
:sparkler:
:wind_chime:
:rice_scene:
:jack_o_lantern:
:ghost:
:santa:
:christmas_tree:
:gift:
:bell:
:no_bell:
:tanabata_tree:
:tada:
:confetti_ball:
:balloon:
:crystal_ball:
:cd:
:dvd:
:floppy_disk:
:camera:
:video_camera:
:movie_camera:
:computer:
:tv:
:iphone:
:phone:
:telephone:
:telephone_receiver:
:pager:
:fax:
:minidisc:
:vhs:
:sound:
:speaker:
:mute:
:loudspeaker:
:mega:
:hourglass:
:hourglass_flowing_sand:
:alarm_clock:
:watch:
:radio:
:satellite:
:loop:
:mag:
:mag_right:
:unlock:
:lock:
:lock_with_ink_pen:
:closed_lock_with_key:
:key:
:bulb:
:flashlight:
:high_brightness:
:low_brightness:
:electric_plug:
:battery:
:calling:
:email:
:mailbox:
:postbox:
:bath:
:bathtub:
:shower:
:toilet:
:wrench:
:nut_and_bolt:
:hammer:
:seat:
:moneybag:
:yen:
:dollar:
:pound:
:euro:
:credit_card:
:money_with_wings:
:inbox_tray:
:outbox_tray:
:envelope:
:incoming_envelope:
:postal_horn:
:mailbox_closed:
:mailbox_with_mail:
:mailbox_with_no_mail:
:package:
:door:
:smoking:
:bomb:
:gun:
:hocho:
:pill:
:syringe:
:page_facing_up:
:page_with_curl:
:bookmark_tabs:
:bar_chart:
:chart_with_upwards_trend:
:chart_with_downwards_trend:
:scroll:
:clipboard:
:calendar:
:date:
:card_index:
:file_folder:
:open_file_folder:
:scissors:
:pushpin:
:paperclip:
:black_nib:
:pencil2:
:straight_ruler:
:triangular_ruler:
:closed_book:
:green_book:
:blue_book:
:orange_book:
:notebook:
:notebook_with_decorative_cover:
:ledger:
:books:
:bookmark:
:name_badge:
:microscope:
:telescope:
:newspaper:
:football:
:basketball:
:soccer:
:baseball:
:tennis:
:8ball:
:rugby_football:
:bowling:
:golf:
:mountain_bicyclist:
:bicyclist:
:horse_racing:
:snowboarder:
:swimmer:
:surfer:
:ski:
:spades:
:hearts:
:clubs:
:diamonds:
:gem:
:ring:
:trophy:
:musical_score:
:musical_keyboard:
:violin:
:space_invader:
:video_game:
:black_joker:
:flower_playing_cards:
:game_die:
:dart:
:mahjong:
:clapper:
:memo:
:pencil:
:book:
:art:
:microphone:
:headphones:
:trumpet:
:saxophone:
:guitar:
:shoe:
:sandal:
:high_heel:
:lipstick:
:boot:
:shirt:
:tshirt:
:necktie:
:womans_clothes:
:dress:
:running_shirt_with_sash:
:jeans:
:kimono:
:bikini:
:ribbon:
:tophat:
:crown:
:womans_hat:
:mans_shoe:
:closed_umbrella:
:briefcase:
:handbag:
:pouch:
:purse:
:eyeglasses:
:fishing_pole_and_fish:
:coffee:
:tea:
:sake:
:baby_bottle:
:beer:
:beers:
:cocktail:
:tropical_drink:
:wine_glass:
:fork_and_knife:
:pizza:
:hamburger:
:fries:
:poultry_leg:
:meat_on_bone:
:spaghetti:
:curry:
:fried_shrimp:
:bento:
:sushi:
:fish_cake:
:rice_ball:
:rice_cracker:
:rice:
:ramen:
:stew:
:oden:
:dango:
:egg:
:bread:
:doughnut:
:custard:
:icecream:
:ice_cream:
:shaved_ice:
:birthday:
:cake:
:cookie:
:chocolate_bar:
:candy:
:lollipop:
:honey_pot:
:apple:
:green_apple:
:tangerine:
:lemon:
:cherries:
:grapes:
:watermelon:
:strawberry:
:peach:
:melon:
:banana:
:pear:
:pineapple:
:sweet_potato:
:eggplant:
:tomato:
:corn:

**Places**

:house:
:house_with_garden:
:school:
:office:
:post_office:
:hospital:
:bank:
:convenience_store:
:love_hotel:
:hotel:
:wedding:
:church:
:department_store:
:european_post_office:
:city_sunrise:
:city_sunset:
:japanese_castle:
:european_castle:
:tent:
:factory:
:tokyo_tower:
:japan:
:mount_fuji:
:sunrise_over_mountains:
:sunrise:
:stars:
:statue_of_liberty:
:bridge_at_night:
:carousel_horse:
:rainbow:
:ferris_wheel:
:fountain:
:roller_coaster:
:ship:
:speedboat:
:boat:
:sailboat:
:rowboat:
:anchor:
:rocket:
:airplane:
:helicopter:
:steam_locomotive:
:tram:
:mountain_railway:
:bike:
:aerial_tramway:
:suspension_railway:
:mountain_cableway:
:tractor:
:blue_car:
:oncoming_automobile:
:car:
:red_car:
:taxi:
:oncoming_taxi:
:articulated_lorry:
:bus:
:oncoming_bus:
:rotating_light:
:police_car:
:oncoming_police_car:
:fire_engine:
:ambulance:
:minibus:
:truck:
:train:
:station:
:train2:
:bullettrain_front:
:bullettrain_side:
:light_rail:
:monorail:
:railway_car:
:trolleybus:
:ticket:
:fuelpump:
:vertical_traffic_light:
:traffic_light:
:warning:
:construction:
:beginner:
:atm:
:slot_machine:
:busstop:
:barber:
:hotsprings:
:checkered_flag:
:crossed_flags:
:izakaya_lantern:
:moyai:
:circus_tent:
:performing_arts:
:round_pushpin:
:triangular_flag_on_post:
:jp:
:kr:
:cn:
:us:
:fr:
:es:
:it:
:ru:
:gb:
:uk:
:de:

**Symbols**

:one:
:two:
:three:
:four:
:five:
:six:
:seven:
:eight:
:nine:
:keycap_ten:
:1234:
:zero:
:hash:
:symbols:
:arrow_backward:
:arrow_down:
:arrow_forward:
:arrow_left:
:capital_abcd:
:abcd:
:abc:
:arrow_lower_left:
:arrow_lower_right:
:arrow_right:
:arrow_up:
:arrow_upper_left:
:arrow_upper_right:
:arrow_double_down:
:arrow_double_up:
:arrow_down_small:
:arrow_heading_down:
:arrow_heading_up:
:leftwards_arrow_with_hook:
:arrow_right_hook:
:left_right_arrow:
:arrow_up_down:
:arrow_up_small:
:arrows_clockwise:
:arrows_counterclockwise:
:rewind:
:fast_forward:
:information_source:
:ok:
:twisted_rightwards_arrows:
:repeat:
:repeat_one:
:new:
:top:
:up:
:cool:
:free:
:ng:
:cinema:
:koko:
:signal_strength:
:u5272:
:u5408:
:u55b6:
:u6307:
:u6708:
:u6709:
:u6e80:
:u7121:
:u7533:
:u7a7a:
:u7981:
:sa:
:restroom:
:mens:
:womens:
:baby_symbol:
:no_smoking:
:parking:
:wheelchair:
:metro:
:baggage_claim:
:accept:
:wc:
:potable_water:
:put_litter_in_its_place:
:secret:
:congratulations:
:m:
:passport_control:
:left_luggage:
:customs:
:ideograph_advantage:
:cl:
:sos:
:id:
:no_entry_sign:
:underage:
:no_mobile_phones:
:do_not_litter:
:no_bicycles:
:no_pedestrians:
:children_crossing:
:no_entry:
:eight_spoked_asterisk:
:sparkle:
:eight_pointed_black_star:
:heart_decoration:
:vs:
:vibration_mode:
:mobile_phone_off:
:chart:
:currency_exchange:
:aries:
:taurus:
:gemini:
:cancer:
:leo:
:virgo:
:libra:
:scorpius:
:sagittarius:
:capricorn:
:aquarius:
:pisces:
:ophiuchus:
:six_pointed_star:
:negative_squared_cross_mark:
:a:
:b:
:ab:
:o2:
:diamond_shape_with_a_dot_inside:
:recycle:
:end:
:back:
:on:
:soon:
:clock1:
:clock130:
:clock10:
:clock1030:
:clock11:
:clock1130:
:clock12:
:clock1230:
:clock2:
:clock230:
:clock3:
:clock330:
:clock4:
:clock430:
:clock5:
:clock530:
:clock6:
:clock630:
:clock7:
:clock730:
:clock8:
:clock830:
:clock9:
:clock930:
:heavy_dollar_sign:
:copyright:
:registered:
:tm:
:x:
:heavy_exclamation_mark:
:bangbang:
:interrobang:
:o:
:heavy_multiplication_x:
:heavy_plus_sign:
:heavy_minus_sign:
:heavy_division_sign:
:white_flower:
:100:
:heavy_check_mark:
:ballot_box_with_check:
:radio_button:
:link:
:curly_loop:
:wavy_dash:
:part_alternation_mark:
:trident:
:black_small_square:
:white_small_square:
:black_medium_small_square:
:white_medium_small_square:
:black_medium_square:
:white_medium_square:
:black_large_square:
:white_large_square:
:white_check_mark:
:black_square_button:
:white_square_button:
:black_circle:
:white_circle:
:red_circle:
:large_blue_circle:
:large_blue_diamond:
:large_orange_diamond:
:small_blue_diamond:
:small_orange_diamond:
:small_red_triangle:
:small_red_triangle_down:
:shipit:
```
