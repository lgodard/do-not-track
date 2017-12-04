# do-not-track

Accessing the user's preferences in terms of tracking can be slightly complicated. This module simplifies that.

## Install

`npm install --save donottrack`

## Usage

Browser:

```javascript
import doNotTrack from 'donottrack';

// Returns false if the user agrees to being tracked, true otherwise.
const do_not_track = doNotTrack(/* default, if preferences are not set. */ false);
```

Node:

```javascript
import doNotTrack from 'donottrack';

const do_not_track = doNotTrack(req.header('DNT'), false);
```
