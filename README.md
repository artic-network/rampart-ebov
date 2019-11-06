# rampart-ebov
RAMPART protocol folder for EBOV

## Installing
Clone this repository:

```
git clone https://github.com/artic-network/rampart-ebov.git
```

Create conda environment and activate it:

```
cd rampart-artic
conda env create -f environment.yml
conda activate rampart-artic
```

## Running

Create run folder:

```
mkdir [run_name]
cd [run_name]
```

Where `[run_name]` is whatever you are calling todays run (as specified in MinKNOW).

Run RAMPART:

```
rampart --protocol ../rampart-ebov --basecalledPath ~/MinKNOW/data/reads/[run_name]/pass
```

`basecalledPath` should be set to whereever MinKNOW/guppy is going to write its basecalled files.

## Example Data

The directory `example_data` contains some reads from an Ebola virus MinION run to test RAMPART with. To try this:

```
cd rampart/example_data
rampart --protocol ../protocol 
```

The `run_configuration.json` file contains the settings for running this example data.
