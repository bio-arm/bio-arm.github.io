# bio-arm.github.io


# How to build a Bioconductor package

    $ su - biocbuild
    $ export PACKAGE_NAME=<< set the package name here >>
    $ git clone https://git.bioconductor.org/packages/$PACKAGE_NAME
    $ R CMD build --keep-empty-dirs --no-resave-data $PACKAGE_NAME
    $ R CMD check $PACKAGE_NAME_version.tar.gz
    $ R CMD INSTALL $PACKAGE_NAME_version.tar.gz
