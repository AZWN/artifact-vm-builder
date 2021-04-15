Artifact VM Builder
===================

Scripts and configuration to build Debian 10 based amd64 VM images
with Qemu for paper artifacts. The resulting VM has a password-less
user account `artifact` that is logged in automatically on the
console.

Requirements
------------

The scripts require the following software:

- Linux or macOS
- `bash`
- `qemu` with `x86_64` support

Usage
-----

Create the VM as follows:

    ./make-artifact-vm

During installation the installer sometimes complains about download
failure. Choosing `<Retry>` is usually enough to fix these problems.

After the VM is created, run as follows:

    cd artifact-vm
    ./run

Modify the `run` script to adapt VM settings such as memory and
network devices.
