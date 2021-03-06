# Fortnite
A simple to use module for interacting with the FortniteTracker API.

## Install
```
$ npm install fortnite
```
## How to
```js
// require the package
const Fortnite = require('fortnite');
const client = new Fortnite('Your-API-Key');
client.getInfo('zerotwothreezero', 'pc').then(data => console.log(data));
```
**An API key is required to send requests. You can get one by signing up [here](https://fortnitetracker.com/site-api).**
- `username` is required and must be a string.
- `platform` is `pc` by default. Possible platforms are: `pc`, `xbl` `psn`.

## Example Response
```js
Account {
  accountId: 'a69bc052-f1e0-44d9-bbda-38385f565d0b',
  username: 'zerotwothreezero',
  platformId: 3,
  platform: 'pc',
  platformNameLong: 'PC',
  url: 'https://api.fortnitetracker.com/v1/profile/pc/zerotwothreezero',
  lifetimeStats:
   [ Stat { stat: 'top3', value: '2' },
     Stat { stat: 'top5s', value: '1' },
     Stat { stat: 'top3s', value: '2' },
     Stat { stat: 'top6s', value: '2' },
     Stat { stat: 'top12s', value: '10' },
     Stat { stat: 'top25s', value: '12' },
     Stat { stat: 'score', value: '14,048' },
     Stat { stat: 'matchesPlayed', value: '112' },
     Stat { stat: 'wins', value: '1' },
     Stat { stat: 'win', value: '1%' },
     Stat { stat: 'kills', value: '39' },
     Stat { stat: 'kd', value: '0.35' },
     Stat { stat: 'killsPerMin', value: '0.1' },
     Stat { stat: 'timePlayed', value: '11h 32m ' },
     Stat { stat: 'avgSurvivalTime', value: '6m 10s' } ],
  stats:
   { p2:
      { trnRating: [Object],
        score: [Object],
        top1: [Object],
        top3: [Object],
        top5: [Object],
        top6: [Object],
        top10: [Object],
        top12: [Object],
        top25: [Object],
        kd: [Object],
        matches: [Object],
        kills: [Object],
        minutesPlayed: [Object],
        kpm: [Object],
        kpg: [Object],
        avgTimePlayed: [Object],
        scorePerMatch: [Object],
        scorePerMin: [Object] },
     p10:
      { trnRating: [Object],
        score: [Object],
        top1: [Object],
        top3: [Object],
        top5: [Object],
        top6: [Object],
        top10: [Object],
        top12: [Object],
        top25: [Object],
        kd: [Object],
        matches: [Object],
        kills: [Object],
        minutesPlayed: [Object],
        kpm: [Object],
        kpg: [Object],
        avgTimePlayed: [Object],
        scorePerMatch: [Object],
        scorePerMin: [Object] },
     p9:
      { trnRating: [Object],
        score: [Object],
        top1: [Object],
        top3: [Object],
        top5: [Object],
        top6: [Object],
        top10: [Object],
        top12: [Object],
        top25: [Object],
        kd: [Object],
        winRatio: [Object],
        matches: [Object],
        kills: [Object],
        minutesPlayed: [Object],
        kpm: [Object],
        kpg: [Object],
        avgTimePlayed: [Object],
        scorePerMatch: [Object],
        scorePerMin: [Object] } },
  recentMatches:
   [ { id: 16623073,
       accountId: 'a69bc052-f1e0-44d9-bbda-38385f565d0b',
       playlist: 'p2',
       kills: 20,
       minutesPlayed: 240,
       top1: 0,
       top5: 0,
       top6: 0,
       top10: 2,
       top12: 0,
       top25: 12,
       matches: 42,
       top3: 0,
       dateCollected: '2018-02-03T01:00:12.957',
       score: 4925,
       platform: 3 },
     { id: 16623072,
       accountId: 'a69bc052-f1e0-44d9-bbda-38385f565d0b',
       playlist: 'p9',
       kills: 4,
       minutesPlayed: 91,
       top1: 1,
       top5: 0,
       top6: 2,
       top10: 0,
       top12: 0,
       top25: 0,
       matches: 11,
       top3: 2,
       dateCollected: '2018-02-03T01:00:12.91',
       score: 2158,
       platform: 3 },
     { id: 16623071,
       accountId: 'a69bc052-f1e0-44d9-bbda-38385f565d0b',
       playlist: 'p10',
       kills: 15,
       minutesPlayed: 361,
       top1: 0,
       top5: 1,
       top6: 0,
       top10: 0,
       top12: 10,
       top25: 0,
       matches: 59,
       top3: 0,
       dateCollected: '2018-02-03T01:00:12.8',
       score: 6965,
       platform: 3 } ] }
```
