## Video Conversion for Laramie Festival
This project is designed to convert video files to meet the specific format requirements of the Laramie Festival. It includes functionality to check video properties and generate a report for any videos that do not conform to the required specifications. Additionally, it provides a script to convert videos to the correct format using ffmpeg.

### Table of Contents
Video Conversion for Laramie Festival
Table of Contents
Description
Installation
Usage
Checking Video Formats
Converting Videos
Example Output
Contributing
License
Description
This project helps ensure that videos meet the Laramie Festival's format requirements. It performs the following tasks:

Checks video properties such as codec, resolution, frame rate, aspect ratio, bitrate, and duration.
Generates a report listing any videos that do not meet the specified requirements.
Converts videos to the correct format using ffmpeg.
Installation
Clone the repository:

git clone https://github.com/yourusername/laramie-festival-video-conversion.git
cd laramie-festival-video-conversion
Install the required dependencies:

pip install -r requirements.txt
Ensure you have ffmpeg installed on your system. You can download it from ffmpeg.org.

Usage
Checking Video Formats
To check the formats of your videos and generate a report:

Place your video files in the Films directory.
Run the script to check the formats:

python check_formats.py
This will generate a report file named format_check_report.txt in the project directory, listing any videos that do not meet the required specifications.

Converting Videos
To convert videos to the correct format:

Place your video files in the Films directory.
Run the conversion script:
bash
Copy code
python convert_videos.py
The converted videos will be saved in the Films directory with the suffix _formatOK added to their filenames.

#### Example Output

Hey there!
As you specified in the documentation, here are your wrong format cells!
In the notebook we dealt with the problem using required formats using interesting functions ;))
Films with incorrect format:
The_Gun_and_the_Pulpit.avi: {'video_name': 'The_Gun_and_the_Pulpit.avi', 'video_codec': 'rawvideo', 'resolution': (720, 'x', 404), 'frame_rate': '25/1', 'aspect_ratio': 'N/A', 'video_bitrate': '87438878', 'video_Format': '.avi'}
...
Conversion
css

Converted Cosmos_War_of_the_Planets.mp4 to Films/Cosmos_War_of_the_Planets_formatOK.mp4
Converted The_Gun_and_the_Pulpit.avi to Films/The_Gun_and_the_Pulpit_formatOK.mp4
...
