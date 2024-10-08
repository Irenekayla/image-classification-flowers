# image-classification-flowers
Part 1 and 2 udacity nanodegree final project submission
Use code with caution.
Markdown
└── train.py
└── predict.py
└── utils.py

## Dependencies

* Python 3
* PyTorch 
* torchvision 
* NumPy
* Pillow (PIL)
* JSON
* (Optional) CUDA-enabled PyTorch (for GPU training)

## Usage

**1. Training:**
```bash
python train.py <data_directory>
Options:

--save_dir <checkpoint_directory> (default: './')

--arch <model_architecture> (choices: 'resnet50', 'vgg13' - default: 'resnet50')

--learning_rate <learning_rate> (default: 0.001)

--hidden_units <hidden_units> (default: 1024)

--epochs <epochs> (default: 5)

--gpu (use GPU for training)

2. Prediction:

python predict.py <image_path> <checkpoint_path>
Use code with caution.
Bash
Options:

--top_k <top_k> (default: 5)

--category_names <category_names_json> (path to JSON file)

--gpu (use GPU for inference)

Example Commands:

# Training (using VGG13 on GPU)
python train.py flowers/ --arch vgg13 --learning_rate 0.003 --epochs 20 --gpu

# Prediction (using a saved checkpoint)
python predict.py flowers/test/1/image_06734.jpg checkpoints/checkpoint_vgg13.pth --top_k 3 --category_names cat_to_name.json --gpu
Use code with caution.
Bash
Contributing
Contributions are welcome! Please open an issue or a pull request to suggest changes.

License
This project is licensed under the MIT License.

**5. Push to GitHub**

* **Stage `README.md`:** Add the README file to the staging area:

   ```bash
   git add README.md
Use code with caution.
Commit: Commit the README file:

git commit -m "Added README.md"
Use code with caution.
Bash
Push: Push your changes to GitHub:

git push origin master
