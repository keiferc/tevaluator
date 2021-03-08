# tevaluator

An object-oriented Python 3 package containing classes for evaluating 
technologies. Used for operations research.

Available modules:

- `tevaluator.tevaluator`: Contains class `Tevaluator`, which holds methods for
  conducting comparative analyses on collections of `Tech` instances. I.e.
  `Tevaluator` is used for analyzing specific collections of technologies 
  through their associated datapoints.
- `tevaluator.tech`: Contains class `Tech`, which holds methods for analyzing 
  `Evaluation` instances for a specific technology. I.e. `Tech` is used to 
  represent a singular piece of technology, containing information about the 
  technology as well as its evaluations.
- `tevaluator.evaluation`: Contains class `Evaluation`, which holds methods for
  operating on `Metric` instances. I.e. `Evaluation` functions as a collection 
  of metrics that collectively represent an idea (e.g. the use case 
  satisfiability of a technology).
- `tevaluator.metric`: Contains class `Metric` and subclasses `Delta` and 
  `Ility`. Used for qualifying `Rating` instances. I.e. `Metric` represents an 
  idea that can be measured.
- `tevaluator.rating`: Contains class `Rating`. Used to collect a source's 
  (e.g. a user) rating for a specific metric being measured. I.e. `Rating` 
  represents a datapoint for a metric (e.g. 3 out of 5 stars).


## Requirements

- Python 3
- pip3
- [`simpleds`](https://github.com/keiferc/simpleds)


## Installation

```bash
$ pip3 install git+https://github.com/keiferc/tevaluator.git
```

Run `pip3 uninstall tevaluator` to uninstall `tevaluator`.


## Development

To install manually:

```bash
$ git clone https://github.com/keiferc/tevaluator.git
$ cd tevaluator
$ python3 -m venv venv # we recommend using a virtual environment
$ source venv/bin/activate
$ make install
$ make clean
```

Run `pytest` to run automated testing.

Run `pip3 uninstall tevaluator` to uninstall `tevaluator`.


## Documentation

Documentation is built using `mkdocs`. More information coming soon.
