# BraiinsOS Power Target No Restart Fix

This branch contains a fix for setting power targets on BraiinsOS miners without causing a restart.

The fix is implemented by using a modified version of the pyasic library from a fork that addresses the restart issue in the BraiinsOS backend.

## Implementation

The only change in this branch is in `requirements.txt`, which now points to a specific branch of a forked pyasic repository instead of using the PyPI version. 