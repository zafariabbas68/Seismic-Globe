
# Seismic Globe

![Seismic Globe](images/frame_649.png)

## Overview

**Seismic Globe** is a data visualization project that maps earthquake events from 2020 to 2024 on a rotating 3D globe. The project fetches earthquake data from the USGS API, processes it, and generates an interactive 3D globe to visualize the earthquakes' location, magnitude, and depth. The globe can be viewed in real-time.

## Features

- **Global Earthquake Data**: Fetches earthquake data (magnitude 5.0 and above) from the USGS Earthquake API.
- **3D Globe Visualization**: Interactive globe that shows earthquake activity over time.
- **Magnitude-based Marker Sizing**: Earthquake markers' size is dynamically scaled based on their magnitude.
- **Depth-based Coloring**: The color of earthquake markers reflects the depth of each earthquake.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/zafariabbas68/Seismic-Globe.git
   ```

2. Navigate to the project directory:
   ```bash
   cd Seismic-Globe
   ```

3. Install the required Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Dependencies:
- `pandas`: For handling the earthquake data.
- `requests`: To fetch data from the USGS API.
- `plotly`: For creating the interactive 3D globe visualization.
- `imageio`: To create animations (if needed).

## Usage

### Step 1: Fetch Earthquake Data

Run the script to fetch the data:
```bash
python fetch_earthquake_data.py
```

This will save the earthquake data in a CSV file (`earthquake_data_2020_2024.csv`).

### Step 2: Visualize Earthquake Data

To visualize the earthquake data on the 3D globe, run the visualization script:
```bash
python visualize_earthquakes.py
```

This will open an interactive Plotly plot in your browser, displaying the earthquakes on a rotating globe.

## File Structure

```
/Seismic-Globe
│
├── /images/              # Directory containing visualization images
├── earthquake_data_2020_2024.csv # Fetched earthquake data saved in CSV format
├── fetch_earthquake_data.py  # Script to fetch earthquake data from the USGS API
├── visualize_earthquakes.py  # Script to generate the 3D globe visualization
├── requirements.txt         # Python dependencies
├── README.md                # Project documentation
└── .gitignore               # Git ignore file
```

## Requirements

The following Python packages are required to run the project:

- `pandas`
- `requests`
- `plotly`
- `imageio`

You can install them using `pip`:

```bash
pip install pandas requests plotly imageio
```

## Contributing

Feel free to open issues and pull requests. Contributions are welcome to improve this project!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **USGS Earthquake API**: For providing the earthquake data used in this project.
- **Plotly**: For their excellent library to visualize geographical data in 3D.
- **Imageio**: For enabling the creation of animations from image frames.
```
