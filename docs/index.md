# RSRT-AlphaFold-Server Documentation

!!! note

    Backup is not yet configured. In an event of file system collapse, your data is at risk.


Welcome to the documentation for the Linux server dedicated to running AlphaFold2-multimer, a powerful tool for predicting protein structures. This server was generously donated to the [Rett Syndrome Research Trust (RSRT)](https://reverserett.org/) and is specifically intended to support Rett Syndrome research in [Bird Lab](https://www.ed.ac.uk/biology/groups/bird) and [Cobb Lab](http://www.cobblab.science/) at the University of Edinburgh. 

Rett Syndrome is a rare genetic neurological disorder that affects brain development, leading to severe cognitive and physical impairments. By leveraging [AlphaFold2-multimer](https://github.com/google-deepmind/alphafold) [@Evans2021.10.04.463034], researchers aim to uncover critical insights into the protein-protein interactions implicated in Rett Syndrome pathology.

## Login

To access (1) `rsrt-af-server` using your UUN:
{ .annotate }

1.  If you require access, please contact `kashyap(dot)c(at)ed(dot)ac(dot)uk`

```bash
ssh <UUN>@rsrt-af-server.bio.ed.ac.uk
```

## File and I/O Management

### Summary of available filesystems


| Directory | Explanation |
| ---- | ---- |
| `/home/<UUN>`| User home directory on SSD volume |
| `/home/shared` | Shared folder on SSD volume |
| `/storage/` | Shared HDD volume |


## AlphaFold

### Genetic databases and model parameters

For easier access, the genetic databases are downloaded and stored here:

```bash
/home/shared/alphafold/database
```

### Software management and installation

Please install using [`conda`](https://github.com/conda-forge/miniforge) and configure packages as per your needs. (1)
{ .annotate }

1.  If you require additional support, please contact `kashyap(dot)c(at)ed(dot)ac(dot)uk`
