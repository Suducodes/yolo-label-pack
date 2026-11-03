# YOLO Label & Pack

Teach a computer to see, with nothing to install.

1. **Label** photos right in your browser: <https://suducodes.github.io/yolo-label-pack/>
2. **Export** your labeled photos as a ready-to-train dataset (`my_dataset.zip`).
3. **Train** your own YOLO model in Google Colab: [Open the notebook](https://colab.research.google.com/github/Suducodes/yolo-label-pack/blob/main/YOLO_Workshop.ipynb)

Built for the BME YOLO workshop (KPR Institute of Engineering and Technology).

## Use your own photos
Click **Use my own photos** at the top: choose photos (or a `.zip` of photos), type the names of the things you want to find, and label away. If your zip is already labeled in YOLO format, its boxes and names load automatically.

## How it works
- `index.html` is a single page that runs entirely in your browser. Your boxes stay on your laptop (saved in your browser, never uploaded).
- The export is a standard YOLO dataset: `images/`, `labels/` (one `.txt` per photo: `class x y width height`) and `data.yaml`. Any YOLO tool can train on it.
- `YOLO_Workshop.ipynb` loads that zip, trains with [Ultralytics YOLO](https://docs.ultralytics.com), scores the model, and lets you download `best.pt`: your trained model.

## Credits
Built-in photos are a small subset of Ultralytics' *African-wildlife* dataset (AGPL-3.0).
