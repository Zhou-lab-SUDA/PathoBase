# PathoBase
An open database for storing and processing the genomes of multiple pathogens, providing genomic information including dcgMLST typing[^ref1], genome annotation, and plasmid prediction.

## Quick Start
PathoBase is a database built upon the foundation of the earlier [EnteroBase](https://enterobase.warwick.ac.uk/)[^ref2], operated and maintained by the research group of Prof. Zhemin Zhou at Soochow University. It is a fully web-based centralized database, and [Google Chrome](https://www.google.com/chrome/) is recommended for access. PathoBase shares the same usage logic as EnteroBase. Therefore, if you have previously used EnteroBase, you should find PathoBase quite familiar.  

The homepage of PathoBase displays available bacterial databases (currently including *A. baumannii*, *A. pittii*, and *S. aureus*) along with an overview of the corresponding bacterial genome counts. You can click on any database to access genomic information for the selected pathogen. However, guest accounts cannot download genome assembly results or create GrapeTree visualizations. We strongly recommend registering and logging in to unlock the full functionality of PathoBase. Let's start with account registration:  

### Registration  
Click the **Register** button in the upper-right corner of the homepage. In the pop-up window, fill in your username, password, email address, and personal information. After completing the required fields, click **Register**. A verification email will be sent to your provided email address. Follow the verification link in the email to complete registration and log in to PathoBase.  

### Login  
Users with existing accounts or those accessing PathoBase via verification credentials can log in by clicking the **Log In** button. Enter your username and password to access most content of PathoBase. We provide a brief tutorial for first-time users, or you may explore the database structure, analysis workflows, and the **dcgMLST + HierCC**[^ref3] algorithm independently. 

## Tutorial based on a simple case
PathoBase excels in storing genomes and clustering newly deposited genomes using **dcgMLST + HierCC**, making it particularly effective in identifying epidemiological associations between strains. We will guide you step by step through an actual example to help you master the basic functionalities of PathoBase.

### *Acinetobacter pittii*

The first part of our tutorial covers genome upload. After logging in and selecting the target pathogen database, you will see the **Upload Reads** option on the left sidebar. Clicking this will direct you to the metadata entry page (if errors occur, refresh the page). Here, you must provide metadata for your genome. We require minimal but informative sample details (e.g., isolation date and country) to assist other users.  

By default, only **raw sequencing reads** (not pre-assembled genomes) are allowed for upload to minimize analytical variability. **Trusted users** may upload assembled genomes. After completing the metadata fields, switch to the data upload page by clicking the **Upload Data** tab. Select the folder containing your data files and click **Upload** to initiate the process. Track progress via the **Job List**, where you can click the task ID for real-time status updates.  
Once analysis concludes, your genome will be integrated into PathoBase. To view all genomes for a species, navigate to its database page and click **Search Strains** > **All Strains**.  

Our *A. pittii* repository includes **xxx preloaded example genomes** from our cgMLST study (see **Supplementary Table X**). These span **x years** and **x countries**, covering **x distinct HC1100s** (see **dcgMLST + HierCC** analysis).  
Return to **Search Strains** and apply filters based on your uploaded genome's metadata. In addition to basic details, the right-side dropdown menu will display population assignments from **cgMLST + HierCC**. For *A. pittii*, two hierarchical clusters are defined: **HC450** and **HC1100**. We recommend starting with **HC1100**.  

Each genome is assigned an integer HC1100 value. Reapply the **Search Strains** filter under **Experimental Data** to select genomes sharing your strain's HC1100 value. This retrieves evolutionarily closely related genomes.  


###



## References
[^ref1]: https://doi.org/10.1038/s41467-023-43528-0
[^ref2]: https://doi.org/10.1093/nar/gkae902
[^ref3]: https://doi.org/10.1093/bioinformatics/btab234
