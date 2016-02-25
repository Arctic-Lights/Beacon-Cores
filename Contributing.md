# Contributing

Thanks for coming out! If you're interested in helping out with the project, there's a few things that you are going to need to know. Be sure to read *everything* before you begin contributing to the project. 

The project is licensed under the Apache 2.0 license, a highly permissive license that allows use within other open source and proprietary projects. It's a popular and trustworthy license, maintained by the Apache Software Foundation. Numerous projects, such as Apple's Swift programming language, are licensed under the Apache 2.0 license.

There's a few guidelines when making code contributions. We aim to make most of the projects machine-readable, so that they can be packaged and processed easily. Since each individual core can be written in any language, this presents a challenge: how can we efficiently read each core's properties? As a result, we need to create a guideline in which to keep information for each individual core.

### Code guidelines

All the cores will be stored in a top-level directory called `/builds`. Each individual core will be given an id, which the core will be located in. Each one will have the running files needed to make the core, as well as a few additional files: a text file contains a checksum for the core's code, and a specialized properties file (`__init__.py`), with details of the core. This will be a python file - an API for reading each core will be made as well. The directory of a build may roughly look like this:

    /builds
    	/files
    		/all_the_other_files.whatever
        /checksum.txt
        /license.txt
        /__init__.py
        
### Code specifications

Since these cores aren't "standalone" executable files that can be run by the end user on their own, they will likely have to communicate with a high-level application, or either on the command line. Therefore, a communication standard/protocol needs to be developed, in order to update and change settings at runtime, or a user setting to be applied for all runtimes.

Code can be written in any language. It can vary from things such as Python, to C, but we prefer that all code and cores have as little dependencies as necessary. While something written in Java or Python might work great, they require things that may not necessarily be automatically present on a user's computer, namely the Java Runtime Environment, or the Python runtime. 


### `__init__.py`

This will be mostly a series of properties containing information, most notably details concerning the names, compatible systems, authors, language, development status as well as a bunch of other parameters. An example is included in the example core. Python was chosen here, since it is simple, and easy to place information within.



##### Frequently Asked Questions:

###### Under what license do I contribute?
Your contributions will be licensed under the Apache 2.0 license. This is in line with the license of all files within the repository.
