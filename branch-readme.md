# Braiins OS+ Power Target No Restart

This branch modifies the Miner integration to use a custom fork of the `pyasic` library that allows changing power target limits without requiring a miner restart.

## Changes Made

1. Modified the integration to install `pyasic` directly from GitHub repository instead of from PyPI.
2. Set the `PYASIC_VERSION` to track the `bosminer-api-power-target` branch.
3. Updated all import statements to use the GitHub version of `pyasic`.
4. Removed references to the non-existent `local_pyasic` module.

## How It Works

The forked `pyasic` library includes modifications to the Braiins OS+ API handler that allows setting power target values without triggering a miner restart. This provides a smoother experience for Home Assistant users who want to adjust power limits without interrupting mining operations.

## Installation

This version will automatically install the proper version of `pyasic` from GitHub when the integration is loaded in Home Assistant.

## Credits

The fix is based on the work of the Upstream Data team and their pyasic library. 