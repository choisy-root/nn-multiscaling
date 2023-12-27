# Model Runner for Build, Approximation, Fine-tuning, and Querying

This Python script acts as a runner for various model operations such as building, approximation, fine-tuning, and querying within a machine learning workflow.

## Features

- Build: Construct models from scratch.
- Approximation: Create approximate versions of the models.
- Fine-tuning: Optimize pre-trained models.
- Querying: Retrieve information about the models.

## Requirements

- TensorFlow
- Horovod for distributed training
- Bespoke (a custom module for machine learning workflows)
- NNCompress (a custom module for neural network compression)

## Usage

Run the script from the command line, providing the necessary arguments:

```bash
python runner.py --config path/to/config.yaml --mode [mode] --source_dir path/to/source --target_dir path/to/target
```

Available modes include:
- `build`
- `approx`
- `finetune`
- `query`
- `transfer_learning`
- `profile`

## Arguments

- `--config`: Path to the configuration file.
- `--mode`: Operation mode.
- `--source_dir`: Working directory path.
- `--target_dir`: Result directory path.
- Additional arguments are available for specific operations.

## Configuration

The script is configured via a YAML file which includes parameters such as dataset paths, model architecture, training settings, etc.

## Customization

You can customize the runner script by adding new modes or modifying the existing workflow to suit different machine learning tasks.

## Contributing

To contribute to the development of this runner script, you can extend its capabilities or improve the existing code to increase efficiency and performance.