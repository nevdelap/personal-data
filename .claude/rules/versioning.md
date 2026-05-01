---
description: Check git tags to decide if version bump is needed
---

# Versioning

After every non-documentation change, bump the patch version in `index.html`:

```html
<div class="subtitle">v0.0.3</div>
```

The major and minor versions are permanently 0.0. Only the patch increments: 0.0.1, 0.0.2, 0.0.3 … 0.0.401 and so on. Every commit gets its own bump — do not skip or share bumps across commits.
