#YouTube Video Downloader
Description
This project is a simple YouTube video downloader built using FastAPI for the backend and HTML/CSS/JavaScript for the frontend. Users can paste a YouTube video URL and select the quality of the video they wish to download.

## Features
- **Paste a YouTube URL to fetch video information.**
- **Select the desired video quality before downloading.**
- **Fast and efficient video downloading using `yt-dlp`.**
- **User-friendly interface.**


Technologies Used
Backend: FastAPI
Frontend: HTML, CSS, JavaScript
Video Downloading: yt-dlp
Python: v3.x

Requirements
Python 3.x
FastAPI
yt-dlp
Uvicorn (for running the FastAPI app)
Installation

Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/youtube-video-downloader.git
cd youtube-video-downloader
Create a virtual environment (optional but recommended):

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

Install the required packages:
bash
Copy code
pip install fastapi yt-dlp uvicorn
Usage

Start the FastAPI server:
bash
Copy code
uvicorn app:app --reload
This will run the backend server on http://127.0.0.1:8000.

Open the index.html file in your web browser.

Paste the YouTube URL into the input box and click the "Fetch Video Info" button.

Select the desired video quality and click "Download".

The video will start downloading based on the selected quality.

API Endpoints
POST /fetch_video_info: Accepts a JSON object containing the YouTube URL and returns available video formats and qualities.

GET /download_video: Accepts the URL and selected quality to download the video.

Troubleshooting
If you encounter issues fetching video information, ensure that the URL is valid and the backend is running correctly.
Check your browser's console for any error messages.
License
This project is licensed under the MIT License.

Author
Your Name
Your Email (optional)
Your GitHub Profile (optional)
