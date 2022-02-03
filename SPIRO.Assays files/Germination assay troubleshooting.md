## SPIRO seed germination assay troubleshooting
| Issue                                                    | Probable cause       | Solution    | 
| ------------------------------------------------------------ | --------------- | ----------- | 
| Seeds are not recognized | Seeds are too large/small | Edit upper/lower area thresholds in cleanup_germination_data.R | 
| Analysis/QC fails with inexplicable errors | Data was edited using Microsoft Excel | Do not edit data using Microsoft Excel |
| Script complains about unused connections | No cause for alarm | Just ignore it |
| Germination processing results look wrong | Something wrong with image analysis | Inspect the 'germinationlabelled.tif' file in the appropriate group folder for errors |
| There is no package called 'pacman' | pacman not installed | `install.packages("pacman")` |
| Results seem to be wrong | Incorrect seed detection parameters | Seeds are not being reliably detected. Tune parameters using [debug mode](https://github.com/jiaxuanleong/SPIRO.Assays#spiro-assay-debug-mode). |
| Unexpected errors from R scripts | Outdated packages | Update your R packages (e.g., `update.packages(ask=F)`) |
| `Error in makePSOCKcluster` | Bug in R on Mac | Update R to version 4.1.2 or higher |
