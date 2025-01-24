

# Seismic Globe  

## Overview  

**Seismic Globe** is a data visualization project that maps earthquake events (2020–2024) on a rotating 3D globe. It fetches earthquake data from the USGS API, processes it, and generates an interactive globe to visualize the earthquakes' locations, magnitudes, and depths. A 30-second animation highlights global earthquake activity with a rotating perspective.  

---

## Features  

- **Global Earthquake Data**: Retrieves earthquake data (magnitude ≥ 5.0) from the USGS Earthquake API.  
- **Interactive 3D Globe**: Displays earthquake events with real-time interactivity.  
- **Magnitude-Based Marker Sizing**: Adjusts marker size dynamically according to earthquake magnitude.  
- **Depth-Based Coloring**: Uses marker colors to indicate earthquake depths.  
- **Rotating Globe Animation**: Produces a 30-second animation showcasing worldwide earthquake activity.  
- **Data Export**: Saves fetched earthquake data as a CSV file for further analysis.  

---

## Installation  

Follow these steps to set up the project:  

1. **Clone the Repository**:  
   ```bash  
   git clone https://github.com/zafariabbas68/Seismic-Globe.git  
   ```  

2. **Navigate to the Project Directory**:  
   ```bash  
   cd Seismic-Globe  
   ```  

3. **Install Required Dependencies**:  
   ```bash  
   pip install -r requirements.txt  
   ```  

### Dependencies  

- `pandas`: For earthquake data processing.  
- `requests`: To fetch earthquake data from the USGS API.  
- `plotly`: To create the interactive 3D globe visualization.  
- `imageio`: To generate animations from image frames.  

---

## Usage  

### Step 1: Fetch Earthquake Data  

The script fetches earthquake data for the years 2020–2024 (magnitude ≥ 5.0) from the USGS Earthquake API.  

Run the following command to fetch and save data as a CSV file:  
```bash  
python fetch_earthquake_data.py  
```  
This will generate `earthquake_data_2020_2024.csv`.  

### Step 2: Visualize Earthquake Data  

To create an interactive 3D globe visualization:  
```bash  
python visualize_earthquakes.py  
```  
This opens a Plotly plot in your browser, displaying earthquake events on a rotating globe.  

### Step 3: Generate an Animation  

To produce a 30-second animation of the rotating globe with earthquake data:  
```bash  
python generate_animation.py  
```  

---

## Animation Preview  

The animation (Earthquake_Globe_Animation.mp4) showcases global earthquake activity:  

[**Download the Animation**](https://github.com/zafariabbas68/Seismic-Globe/raw/main/Earthquake_Globe_Animation.mp4)  

---

## File Structure  

```  
/Seismic-Globe  
│  
├── /frames/                   # Directory for animation frames  
├── earthquake_data_2020_2024.csv  # Fetched earthquake data in CSV format  
├── Earthquake_Globe_Animation.mp4 # Final animation of the rotating globe  
├── fetch_earthquake_data.py      # Script to fetch earthquake data from the API  
├── visualize_earthquakes.py      # Script to create the 3D globe visualization  
├── generate_animation.py         # Script to generate the animation  
├── requirements.txt              # Python dependencies  
├── README.md                     # Project documentation  
└── .gitignore                    # Git ignore file  
```  

---

## Requirements  

Ensure the following Python packages are installed:  

- `pandas`  
- `requests`  
- `plotly`  
- `imageio`  

Install these dependencies using:  
```bash  
pip install pandas requests plotly imageio  
```  

---

## Contributing  

Contributions are welcome! Feel free to submit issues and pull requests to improve the project.  

---

## License  

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.  

---

## Acknowledgments  

- **USGS Earthquake API**: For providing earthquake data.  
- **Plotly**: For their interactive visualization library.  
- **Imageio**: For enabling animation creation from image frames.  

