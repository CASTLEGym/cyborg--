# Cyborg-- Emulation Configuration

## Files to Store or Replace

- Place the `scenario2_cyborg--` file in the `scenario` directory of Cyborg.
- Replace the `linux_user_host_image1` file in the `image` folder of Cyborg with the new image file.

## Changes in the Training Script

- Update your training script to point to the new scenario file `scenario2_cyborg--`.
- The action space for the blue team has been reduced from 145 to 144 due to the reduced action space. Update the action space in your training script accordingly. Use the provided enumerated action list for scenario2 (`blue_enum_action.txt`) or for the modified scenario (`blue_enum_action_cyborg--.txt`) to select the appropriate action space.
- For the Cardiff agent, decrease all actions by 1 in the training script to align with the updated action space.


## Changes in the Evaluation Scripts

- Update your evaluation script  (evaluation.py)to point to the new scenario file `scenario2_cyborg--`.
-  If you are using cardiff_uni structure, since the action space for the blue team has been reduced from 145 to 144 due to the reduced action space, we need to update the action space in your `MainAgent.py' script accordingly. Modified evalaution script and MainAgent script can be downloaded. 
