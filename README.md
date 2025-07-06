# Buildkite Input Step Example

[![Build status](https://badge.buildkite.com/a947f64837044296a1ea4394819872e0544a4647a3400e6634.svg?branch=main)](https://buildkite.com/buildkite/input-step-example)
[![Add to Buildkite](https://img.shields.io/badge/Add%20to%20Buildkite-14CC80)](https://buildkite.com/new)

This repository is an example [Buildkite](https://buildkite.com/) pipeline that demonstrates how to use an [Input Step](https://buildkite.com/docs/pipelines/configure/step-types/input-step) to pause a build and request manual input.

👉 **See this example in action:** [https://buildkite.com/docs/pipelines/input-step-example](https://buildkite.com/buildkite/input-step-example/builds/latest)

See the full [Getting Started Guide](https://buildkite.com/docs/guides/getting-started) for step-by-step instructions on how to get this running, or try it yourself:

[![Add to Buildkite](https://buildkite.com/button.svg)](https://buildkite.com/new)

<p align="left">
  <img src=".buildkite/screenshot-1.png" alt="Input step screenshot" width="600" />
  <br>
  <em>The pipeline paused at an input step</em>
</p>

<p align="left">
  <img src=".buildkite/screenshot-2.png" alt="Popup dialog for input" width="600" />
  <br>
  <em>The input dialog prompting for a value</em>
</p>

<p align="left">
  <img src=".buildkite/screenshot-3.png" alt="Build after input submission" width="600" />
  <br>
  <em>The pipeline resuming after the input is submitted</em>
</p>

<p align="left">
  <img src=".buildkite/screenshot-4.png" alt="Script output using input" width="600" />
  <br>
  <em>The input value echoed back by the script</em>
</p>

<!-- docs:start -->

## How it works

This example:
- Uses an [Input Step](https://buildkite.com/docs/pipelines/input-step) to ask for a value mid-pipeline.
- Passes that value to a script (choose from [`script.sh`](script.sh) or [`script.ps1`](script.ps1)) that echoes it back.
- Can be extended to support manual approvals, environment switching, or conditional builds.

To switch platforms, edit the step in `.buildkite/pipeline.yml`.

<!-- docs:end -->

## License

See [Licence.md](Licence.md) (MIT)
