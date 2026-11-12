# Data Roundtrip with `qim3d`, `gvxr`, and `cil`

This collection of notebooks can be used to achieve a full in-sillica XCT experiment:

1. `qim3d`: Generate a dataset
    - Generate a twisted rope made of N strands using `qim3d.generate.rope`
2. `gvxr`: Simulate experiment to produce projections
    - Assign differenet metals and plastic material properties to the rope strands
    - Produce dataset with either low-noise or high-noise scenario
3. `cil`: Reconstruct the data
    - Reconstruct using FDK
    - Reconstruct using iterative method (FISTA) and TV regularisation
4. `qim3d` (TODO): Segment the data and compare against generated ground truth

## Getting an environment
An appropriate environment for use on Linux can be (reproducibly!) made using `pixi` and the `pyproject.toml` + `pixi.lock` files in this directory. 

You can install `pixi` by running:
```sh
curl -fsSL https://pixi.sh/install.sh | sh
```

Then you can install the environment with `pixi install` and then launch jupyter with `pixi run jupyter lab`

NOTE: This is not fully finished or polished to the extent that one (such as myself) would like. Use without caution, but with an abundance of patience.

## Other

You may be interested in joining the Qim Community on Discord: https://discord.gg/R7Yp7QNJHy — Come say hello!
