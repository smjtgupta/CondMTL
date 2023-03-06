# Conditional MTL (CondMTL)

Official implementation of ["_Same Same, But Different_: Conditional Multi-Task Learning for Demographic-Specific Toxicity Detection"](https://arxiv.org/pdf/2302.07372.pdf). Accepted at [*The Web Conference 2023*](https://www2023.thewebconf.org/).

---

<p align="center"> 
    <img src="https://github.com/smjtgupta/CondMTL/blob/main/resources/mtl_labels.png" width="450">
</p>

Label contamination occurs in a Traditional MTL label assignment when posts that target a given group (<span style="color:green">**Green**</span>) are assumed
to be non-toxic toward any other group (e.g., <span style="color:orange">**Orange**</span>). <span style="color:red">**Red**</span> denotes
unsupported label assignments, while (<span style="color:blue">**$\cdot$**</span>) correctly denotes that these
posts do not contain a label w.r.t. the <span style="color:orange">**Orange**</span> target group.

---

## Install

```bash
git clone https://github.com/smjtgupta/CondMTL.git
cd ConMTL
pip install -r requirements.txt
```

## Run Experiments

To reproduce experimental results simply run each notebook in the directory. <br>
All the notebooks use a portion of the Wilds: Civil Comments [dataset](https://worksheets.codalab.org/bundles/0x8cd3de0634154aeaad2ee6eb96723c6e). <br>
All the notebooks are named appropriately based on the architecture / loss functions they use.

## Citation

If you use **CondMTL** in your own work, please cite the following paper:

```bib
@inproceedings{gupta-webconf23,
  title = {{{\em Same Same, But Different}: Conditional Multi-Task Learning for Demographic-Specific Toxicity Detection}},
  author = {Soumyajit Gupta and Sooyong Lee and Maria De-Arteaga and Matthew Lease},
  booktitle = {{Proceedings of the Web Conference}},
  year = {2023},
  url = {https://utexas.box.com/shared/static/a6x1y3yisbbqasnr7iqfn5fyht3zyrma.pdf},
  techreport = {https://arxiv.org/abs/2302.07372}
}
```