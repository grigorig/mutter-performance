### Install dependencies

dnf build-dep mutter

dnf install rpm-build rpmdevtools

### Set up environment

rpmdev-setuptree

### Download source tarball

spectool --define "_sourcedir $PWD" -g -R mutter.spec

### Build

rpmbuild --define "_sourcedir $PWD" -ba mutter.spec 

