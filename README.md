# fakewheelofnames

An offline-capable Wheel of Names interface with multiple wheels, persistent entries, synchronized results, sound effects, and local controls.

## Run locally

Open [`src/index.html`](src/index.html) directly in a browser, or serve the repository with any static web server.

The application and its sound effects run without a network connection.

## Predetermine a result

A wheel result can be selected quietly before spinning:

1. Click the segment that should win.
2. No marker or visual effect is shown—the selection stays hidden.
3. Click the white center circle of that same wheel to start the spin.
4. The wheel performs a normal-looking spin and stops on the selected segment.

This works independently on every wheel. Selecting a segment on one wheel does not affect the others.

## Spin speed controls

While wheels are spinning, use these keyboard controls:

| Key | Effect |
| --- | --- |
| **J** | Give wheel 1 a large speed boost |
| **K** | Give wheel 1 a smaller speed boost |
| **I** | Give wheel 2 a large speed boost |
| **L** | Give wheel 2 a smaller speed boost |

A small boost produces a gentler extension than a large boost. Stop pressing boost keys and the wheel resumes its normal deceleration and slows to a stop.

If a result was selected before the spin, boosts add full rotations without changing the selected winner.

## Other controls

- Edit each wheel independently using its Wheel tab and the entries editor.
- Use **Add wheel** to create more wheels.
- Use **Remove wheel** to remove the currently selected wheel; at least one wheel remains.
- Use **Spin all wheels** to spin every wheel and wait for all results before opening the combined winner dialog.
- Open the **Results** tab to view persistent result history for all wheels.

Wheel entries, rotations, wheel count, and result history are saved in local browser storage.