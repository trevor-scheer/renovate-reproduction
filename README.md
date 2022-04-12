This repo demonstrates a semver violation by Renovate. The `@apollo/core-schema` NPM package is currently set to `^0.2.3`. Renovate is configured to group patch/minor updates only on the `renovate/all-npm-minor-patch` branch.

According to semver, packages versioned `0.x.y` are treated as a _major_ bump on `x`, however Renovate is attempting to bump to `^0.3.0` and treat it as a minor.