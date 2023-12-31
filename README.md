# Autodistill with Synthetic Data from DALL-E 2 using LLaMa 2

## Table of Contents

- [Introduction](#introduction)
- [Usage](#usage)
- [Test Results](#test-results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Autodistill with Synthetic Data from DALL-E 2 using LLaMa 2 project is aimed at utilizing synthetic datasets generated by combining the two advanced AI models: DALL-E 2 and LLaMa 2. DALL-E 2 is an image generation model developed by OpenAI, and LLaMa 2 is a language model developed by Meta, capable of generating diverse and creative text prompts. The project's primary goal is to use these text prompts as inputs for DALL-E 2 to create synthetic datasets, which can then be used to train machine learning models, using the Autodistill.

Autodistill uses big, slower foundation models to train small, faster supervised models. Using autodistill, you can go from unlabeled images to inference on a custom model running at the edge with no human intervention in between.

By leveraging synthetic data, we can potentially improve the target model's robustness, reduce the dependency on large-scale real-world data, and enhance the overall training efficiency.

## Usage

1. Preparing the prompts

- Visit [LLaMa 2](https://huggingface.co/spaces/ysharma/Explore_llamav2_with_TGI) to generate creative and diverse text prompts. These prompts will act as inputs for DALL-E 2. Here I've chosen to generate traffic lights dataset.

2. Generate the images

- Go to [DALL-E 2](https://labs.openai.com/) to genreate the images from the prompts given by LLaMa 2.
- Since DALL-E 2 provides around 4 images for each prompt, try using it several times to acquire enough images.
- Download the resultant images and place them in the appropriate directories.

3. [Autodistill](https://github.com/autodistill/autodistill)

- Try the attached notebook for further instructions.
- For the weights file, please check the attached text file in runs folder

## Test Results

I've sourced the test data from [this repo](https://github.com/Thinklab-SJTU/S2TLD). And here are few test results.

![Image 1](./runs/predict/000000.jpg)
![Image 2](./runs/predict/000001.jpg)
![Image 3](./runs/predict/000002.jpg)
![Image 4](./runs/predict/000003.jpg)
![Image 5](./runs/predict/000004.jpg)
![Image 6](./runs/predict/000793.jpg)
![Image 7](./runs/predict/000792.jpg)

## Contributing

Contributions to this project are welcome! If you want to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them with descriptive commit messages.
4. Push your changes to your forked repository.
5. Open a pull request, explaining the changes you made.

Please ensure your contributions align with the project's guidelines and coding standards.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code following the terms and conditions of the license.
