# Global Earthquakes Greater Than 2.5 Magnitude

Source behind https://www.youtube.com/watch?v=Q8Bs7SmFHMM

## Data

Data scraped from USGS on July 7, 2019. Scrape implementation is located at `01_scrape_usgs_data.ipynb`, with output in `data.sqlite3`.

## Rendering

Data processing was done with `pandas` and `numpy` before rendered in `matplotlib`. Robinson map projection was implemented using `mpl_toolkits.basemap`. Frames were stiched together using `ffmpeg`.

The default settings for this render generates ~7200 3040x1920 frames, resulting in 2 minutes of 4K 60fps output. This can be tuned using the parameters in `10_render_frames.ipynb`.


V1 version: https://www.youtube.com/watch?v=IXnJq7yUJoo
