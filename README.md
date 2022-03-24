# @neuenet/extensions

> Lists of [Handshake](https://handshake.org) extensions owned and operated by [Neuenet](https://registry.neuenet/)



## Install

```sh
npm i @neuenet/extensions
```



## Usage

```ts
import extensions, { mature, reserved, sansMature } from "@neuenet/extensions";



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

console.log(reserved);

/*
[
  '07d0eb',      'bchfrnt',
  'beachback',   'beachfront',
  'chronver',    'collectr',
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
- `reserved` exports contains names that are for private use by Neuenet.
- `sansMature` export contains names that are "safe for work."
- Default export combines `mature`, `reserved`,  and `sansMature` exports and sorts alphabetically.
- All names in these lists are Unicode. If converting to punycode, use the transitional mode to ensure validity of your output.



🤝
