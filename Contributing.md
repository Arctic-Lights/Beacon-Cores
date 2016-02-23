# Contributing

Thanks for coming out! If you're interested in helping out with the project, there's a few things that you are going to need to know. Be sure to read *everything* before you begin contributing to the project. 

The project is licensed under the Apache 2.0 license, a highly permissive license that allows use within other open source and proprietary projects. It's a popular and trustworthy license, maintained by the Apache Software Foundation. Numerous projects, such as Apple's Swift programming language, are licensed under the Apache 2.0 license.

There's a few guidelines when making code contributions. We aim to make most of the projects machine-readable, so that they can be packaged and processed easily. Since each individual core can be written in any language, this presents a challenge: how can we efficiently read each core's properties? As a result, we need to create a guideline in which to keep information for each individual core.

### Code guidelines

All the cores will be stored in a top-level directory called `/builds`. Each individual core will be given an id, which the core will be located in. Each one will have the running files needed to make the core, as well as a few additional files: a text file contains a checksum for the core's code, and a specialized properties file, with details of the core. This will be a python file - an API for reading each core will be made as well. The directory of a build may roughly look like this:

    /builds
    	/files
    		/all_the_other_files.whatever
        /checksum.txt
        /properties.py
        
### properties.py

##### Frequently Asked Questions:

###### Under what license do I contribute?
Your contributions will be licensed under the Apache 2.0 license. This is in line with the license of all files within the repository.
