## SPIRO root growth assay troubleshooting
| Issue                                                    | Probable cause       | Solution    | 
| ------------------------------------------------------------ | --------------- | ----------- | 
| Analysis/QC fails with inexplicable errors | Data was edited using Microsoft Excel | Do not edit data using Microsoft Excel |
| Script complains about closing unused connections | No cause for alarm | Just ignore it |
| Script warns that 'giveCsparse' has been deprecated | No cause for alarm | Just ignore it |
| Error: Can't handle an object of class "glmmTMB" | emmeans incompatibility | Try reinstalling emmeans using `install.packages("emmeans")` |
| There is no package called 'pacman' | pacman not installed | `install.packages("pacman")` |
| Results seem to be wrong | Incorrect seed detection parameters | Seeds are not being reliably detected. Tune parameters using [debug mode](https://github.com/jiaxuanleong/SPIRO.Assays#spiro-assay-debug-mode). |
| Results seem to be wrong | Roots are not correctly segmented | Enable overlay skeletons in [debug mode](https://github.com/jiaxuanleong/SPIRO.Assays#spiro-assay-debug-mode). |
| Results seem to be wrong | Other reason | Enable keeping intermediate files in [debug mode](https://github.com/jiaxuanleong/SPIRO.Assays#spiro-assay-debug-mode). These files can be used to determine what is going wrong. |
| Unexpected errors from R scripts | Outdated packages | Update your R packages (e.g., `update.packages(ask=F)`) |
