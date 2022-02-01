# @neuenet/extensions

> Lists of [Handshake](https://handshake.org) extensions owned and operated by [Neuenet](https://neuenet.com)



## Install

```sh
npm i @neuenet/extensions
```



## Usage

```ts
import extensions, { mature, sansMature } from "@neuenet/extensions";



console.log(extensions);

/*
[
  '0451',           '07d0eb',        '0x01',        '2077',
  '247366',         '24hrs',         '2oo',         '50p',
  '5oo',            'abilao',        'acapella',    'acappella',
  'accentuates',    'adamjensen',    'adblockers',  'adults',
  'adza',           'afrobeat',      'afrohaus',    'aihr',
  ... more items
]
*/

console.log(mature);

/*
[
  'adults',      'buttock',
  'buttocks',    'buttsecks',
  'chub',        'creamtube',
  ... more items
]
*/

console.log(sansMature);

/*
[
  '0451',          '07d0eb',        '0x01',           '2077',
  '247366',        '24hrs',         '2oo',            '50p',
  '5oo',           'abilao',        'acapella',       'acappella',
  'accentuates',   'adamjensen',    'adblockers',     'adza',
  'afrobeat',      'afrohaus',      'aihr',           'airhead',
  ... more items
]
*/
```



## Notes

- `mature` export contains potentially offensive, definitely adult language.
- `sansMature` export contains words that are "safe for work."
- Default export combines `mature` and `sansMature` exports are sorts alphabetically.
- All words in these lists are Unicode. If converting to punycode, use the transitional mode to ensure validity of your output.



🤝
