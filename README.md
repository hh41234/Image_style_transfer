# README

## Traditional Style Transfer
- The "Traditional Style Transfer" folder contains two parts of code: one for texture stitching and the other for texture transfer.

- To run the texture stitching code, enter the following command in the command line:

  ```python
  python3 main.py --synthesis -i <path of texture_img> -b <block_size> -o <overlap_size> -t <tolerance>
  ```
  
- To run the texture transfer code, use the following command in the command line:

  ```python
  python3 main.py --transfer -i1 <path of style_img> -i2 <path of content_img> -b <block_size> -o <overlap_size> -t <tolerance> -a <alpha>
  ```

- Apart from the adjustable parameters in the above two commands, other tunable parameters can be explored by running:

  ```python
  python3 main.py -h
  ```

- In addition to the code, the folder also contains `img_style` (style images) and `img_content` (content images) directories for use. The results obtained from running the code are stored in the `output` folder.

## Modern Style Transfer

- The "Modern Style Transfer" folder includes two parts of code: one for regular style transfer with fixed styles (`tran.ipynb`) and another for fast style transfer with fixed styles (`batch_tran.ipynb`).

- In `tran.ipynb`, you can import style images in the second code block and adjust the number of training iterations in the seventh code block. In `batch_tran.ipynb`, the second code block allows importing style images, and the seventh code block allows importing a set of content images. The eleventh code block demonstrates adjustable parameters.

- Besides the code, the folder also contains `img_style` (style images), `img_content` (content images), and the COCO dataset for use. Additionally, there are noise images (`noise.jpg`, `white.jpg`) and pre-computed results stored in the `output` and `loss` folders.


