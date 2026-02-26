.. _whats_new:

###############################
What's New in {Singularity} 4.4
###############################

This section highlights important changes and new features in {Singularity} 4.4
that are of note to users. See also the "What's New" section in the Admin Guide
for administrator-facing changes.

===========
OCI Support
===========

- Correctly escape ENV vars when importing OCI containers to native SIF, so that
  they match podman / docker behaviour.

==============
Native Runtime
==============

- Include the home directory in the ``--workdir`` option (which is a modifier of
  the ``--contain`` option).  This has always been in the ``--workdir`` usage
  description but the home directory has not actually been included at least
  since singularity 2.
- Add ``/etc/resolv.conf`` to the list of host paths that can be prevented
  from automatic import into the container with the ``--no-mount`` option.
