# PathoBase
PathoBase is an open bioinformatics platform for storing, analyzing, and processing microbial pathogen genomes. The database provides comprehensive genomic analysis capabilities, including distributed core genome Multi-Locus Sequence Typing (dcgMLST) [^ref1], automated genome annotation, and advanced plasmid prediction algorithms.

## Quick Start
PathoBase was developed based on the open-source framework of [EnteroBase](https://enterobase.warwick.ac.uk/)[^ref2], and is currently maintained by Professor Zhemin Zhou's research group at Soochow University. As a web-based centralized database, PathoBase is optimized for use with [Google Chrome](https://www.google.com/chrome/) and maintains similar interface logic to EnteroBase, making it immediately familiar to users of that platform.
The PathoBase homepage displays the available bacterial databases—currently featuring *Acinetobacter pittii*, *Acinetobacter baumannii*, and *Staphylococcus aureus*—along with real-time statistics on genome counts for each pathogen. Users can access species-specific genomic information by selecting any of these databases. While limited browsing is available to guest users, full functionality—including genome assembly downloads and GrapeTree visualizations—requires registration and authentication.

### Account Registration

For potential use of Reviewers, we offered a DEMO administrator account:
Account: `zhemin`
Password: `Soochow`

To register for PathoBase:

1.	Click the Register button in the upper-right corner of the homepage
2.	Complete all required fields in the registration form, including username, password, email address, and institutional affiliation
3.	Submit the form by clicking Register
4.	Check your email for a verification message containing an activation link
5.	Follow the verification link to activate your account and gain access to PathoBase

 
Logging In
Users with existing accounts can authenticate by:

1.	Clicking the Log In button
2.	Entering their username and password credentials
3.	Selecting the "Remember me" option (optional) for persistent sessions

First-time users will receive a brief tutorial introducing key features, though experienced users may choose to explore the database structure, analysis workflows, and the dcgMLST + HierCC (Hierarchical Clustering of cgMLST) 3 algorithm independently.


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
