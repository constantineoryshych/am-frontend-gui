# Dev notes

on path ```./src/ts``` create a file```index.dev.ts```, git ignores him, everyone has their own. Webpack uses it as an entry point.

Sample content ```index.dev.ts```:
```typescript
import { Presenters } from "./presenters";

// Import certain Component
import { IndexComposition } from "./components/IndexComposition";

import { render } from "./render";

const presenters = new Presenters();

// Render only specific Component
render(IndexComposition, presenters);
```

Instead **IndexComposition** import any component directly and render it personally
