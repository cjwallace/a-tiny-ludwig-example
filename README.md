# a tiny ludwig example

Just a clone-able, runnable (🤞), minimal example of the [Ludwig](https://uber.github.io/ludwig) low code toolbox.

The example is the Auto MPG example used in the [Ludwig documentation](https://uber.github.io/ludwig/examples/#simple-regression-fuel-efficiency-prediction).
That is itself a recreation of the [basic regression](https://www.tensorflow.org/tutorials/keras/basic_regression) TensorFlow example.
Here, we include the dataset and explicit instructions.

## contents

The `automobiles` directory contains:

- A cleaned csv of the [Auto MPG](https://archive.ics.uci.edu/ml/datasets/auto+mpg) data set. Rows with missing values have had the `?` character from the original dataset removed to avoid parsing errors.
- A model specification file, `model_definition.yaml`.
- A run script with the right Ludwig invocation, `experiment.sh`.

## instructions

Assuming you have a working python3 installation and git on a unix operating system.

- Open a terminal.
- Clone this repo somewhere sensible with `git clone git@github.com:cjwallace/a-tiny-ludwig-example.git`.
- `cd` into the repo.
- Run `python3 -m venv venv`.
- Run `source venv/bin/activate`.
- Run `pip install ludwig`.
- `cd` into the `automobiles` directory.
- Run `./experiment.sh`.
  - If this doesn't work, you may need to run `chmod +x experiment.sh` first to give the script permission to execute.
  - Alternatively, copy the contents of `experiment.sh` and run it on the command line directly.
- Sit back and relax.
