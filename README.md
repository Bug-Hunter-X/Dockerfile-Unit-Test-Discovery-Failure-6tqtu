# Dockerfile Unit Test Discovery

This repository demonstrates a common error in Dockerfiles when running unit tests: failure to properly discover tests when they're located in subdirectories.  The original `Dockerfile` misses crucial steps to ensure that the `unittest` module can find and execute these tests.

The `solution.Dockerfile` provides the corrected Dockerfile that addresses this issue, illustrating the appropriate use of `python -m unittest discover` along with specifying the test directory.