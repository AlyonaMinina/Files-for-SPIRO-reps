## SPIRO data preprocessing troubleshooting
| Issue                                                    | Probable cause       | Solution    | 
| ------------------------------------------------------------ | --------------- | ----------- | 
| Drift correction does not work | The reference point for correction are missing | Do not crop off engravings with SPIRO title and scale bar |
| Drift correction does not work | Either day or night images are too dark or oversaturated | Adjust the shutter speed and rerun the experiment or remove the data from analysis |
| "Not enough RAM" error | The batch size is too big for RAM allocated to ImageJ | Increase RAM. Open Fiji, in the top menu find *Edit -> Options -> Memory and Threads* -> Type in a new RAM value (it typically should be 75% of your computer RAM) |
| "Not enough RAM" error | The batch size is too big for RAM allocated to ImageJ | Reduce the number of images used for each batch. Hold down Ctrl during startup (when prompted) and enter a lower number. |
