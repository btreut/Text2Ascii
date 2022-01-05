# Text2Ascii

CvsClient.mod.cvs has been created by Pieter Muller on 25-Mar-2003 and stored in the SourceForge CVS repository of project [NativeOberon](https://sourceforge.net/projects/nativeoberon/) as ASCII output of itself. Its purpose is to convert Oberon Textfiles to pure ASCII code by creating escape sequences for the non ASCII parts. The reason is that Oberon Textfiles are in no way pure ASCII texts. But they have to be pure ASCII so that they can be handled easily by source code revision systems. Oberon Textfiles may contain formating, active elements (like running clocks or animated pictures), active plots, folds and many things more. These active elements are in general binary objects. Almost all sources of the Oberon System and the compiler were stored as Oberon Textfiles until around 2013/2015. I recovered CvsClient.mod.cvs from the CVS repository and transferred it to this place on 29-Dec-2020. There are only a hand full of places (i.e. in lines 1-3, 4, 430, 432, 447, 449, 559, 561, 948, and 950), where such escape sequences have to be removed manually to create a compilable source. I changed the original name CvsClient to Text2ASCII because I think that CvsClient obscures the relevant usage a bit. There may be more functionality in the code, which I not yet discovered.

More info about the way the binary content is handled can be found in [CvsClient.Mod.cvs](https://github.com/btreut/Text2Ascii/blob/552be57e2324d2feb634ec2d930480953a6d2e29/CvsClient.Mod.cvs#L1012) after line 1012.
