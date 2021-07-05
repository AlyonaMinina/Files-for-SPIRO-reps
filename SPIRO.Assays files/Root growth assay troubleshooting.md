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
| The macro has a built-in method of detecting folders that have not been fully processed and resuming from there. You may make use of this feature by deleting certain files intentionally. Here are the files to delete in case you want to resume from a specific step, for example, error in selecting groups/seedlings or for debugging purposes. |  |    |  | Step 2/6. Finding seedling positions -> X_seedlingpositions.zip Step 3/6 Tracking germination -> X_germination analysis.tsv Step 4/6. Determining start of root for each seedling -> X_rootstartcoordinates.tsv Step 5/6. Processing image to make roots more visible -> X_rootmask.tif Step 6/6. Tracking root growth -> X_rootgrowthdetection.tif |
