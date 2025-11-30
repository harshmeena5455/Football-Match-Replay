# Football Match Replay ⚽🥅

**Top football clubs like Liverpool and Chelsea use tracking data to win matches.** They analyze player movements to perfect tactics, spot weaknesses, and make data driven decisions to improve their overall performance.
This project processes **145K real match frames** from Metrica Sports so you can see exactly how the pros do it, right on your computer.

[![demo.gif](demo.gif)](demo.gif)
<img width="1498" height="1005" alt="Screenshot 2025-11-30 214511" src="https://github.com/user-attachments/assets/8761ea2f-6e2e-4475-8f78-6be359f3ba2b" />


## Features

- **Match Replay Visualization**: Watch 22 players + ball move in real-time on animated pitch
- **Live Player Tracking**: Home (blue) vs Away (red) teams with 145K frames @ 25Hz
- **Interactive Controls**: Pause (SPACE), rewind/fast-forward (←→ arrow keys)
- **Real Match Data**: 96-minute full match from Metrica Sports sample dataset
- **Frame-Accurate Replay**: 25 FPS animation processing 8M+ data points
- **Demo Generator**: `make_demo.py` creates shareable 15s highlight GIFs

## Controls

- **Pause/Resume**: `SPACE`
- **Rewind/Fast Forward**: `←` / `→` arrow keys
- **Restart**: Hold `R`

## Requirements

- Python 3.10+
- [Pandas](https://pandas.pydata.org/) (data processing)
- [Matplotlib](https://matplotlib.org/) (animation)
- [NumPy](https://numpy.org/) (arrays)
- [Pillow](https://pillow.readthedocs.io/) (GIF export)
- [Kloppy](https://kloppy.readthedocs.io/) (sports data)

``pip install -r requirements.txt``

## Usage

Run the interactive replay:

`python main.py`

Generate demo GIF (15 seconds):

`python make_demo.py`


## Customization

- **Pitch dimensions/colors**: `src/arcade_replay.py`
- **Player markers/trails**: `animate()` method
- **Playback speed**: `interval=40` (milliseconds)
- **Demo length**: `range(0, 375, 5)` in `make_demo.py`

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Disclaimer

No copyright infringement intended. Metrica Sports data used for educational purposes only under fair use. All trademarks belong to their respective owners.

---

**Built with ❤️ for football enthusiasts**  
**Data: [Metrica Sports Sample Data](https://github.com/metrica-sports/sample-data)**
