## SPIRO root growth assay troubleshooting
| Issue                                                    | Probable cause       | Solution    | 
| ------------------------------------------------------------ | --------------- | ----------- | 
| Analysis/QC fails with inexplicable errors | Data was edited using Microsoft Excel | Do not edit data using Microsoft Excel |
| Script complains about ununsed connections or NaN's | No cause for alarm | Just ignore it |
| Error: Can't handle an object of class "glmmTMB" | emmeans incompatibility | Try reinstalling emmeans using `install.packages("emmeans")` |
| There is no package called 'pacman' | pacman not installed | `install.packages("pacman") |
