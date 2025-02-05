<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Background Removal - README</title>
</head>
<body>
    <h1>Background Removal Without Deep Learning</h1>
    <p>This project implements background removal using classical image processing techniques such as:</p>
    <ul>
        <li><strong>K-Means Clustering</strong> (Color-Based Segmentation)</li>
        <li><strong>Watershed Algorithm</strong> (Marker-Based Segmentation)</li>
        <li><strong>Graph Cut (GrabCut)</strong> (Foreground Extraction)</li>
    </ul>
    <p>The methodology follows steps inspired by <a href="https://docs.aspose.com/imaging/net/image-masking/#auto-masking" target="_blank">this paper</a>.</p>
    <h2>Example Results</h2>
    <table>
        <tr>
            <th>Input Images</th>
            <th>Output Images</th>
        </tr>
        <tr>
            <td><img src="input1.jpg" alt="Input Image 1" width="300"></td>
            <td><img src="output1.png" alt="Output Image 1" width="300"></td>
        </tr>
        <tr>
            <td><img src="input2.jpg" alt="Input Image 2" width="300"></td>
            <td><img src="output2.png" alt="Output Image 2" width="300"></td>
        </tr>
    </table>
    <h2>How It Works</h2>
    <ol>
        <li>Convert the image to different color spaces (RGB, HSV, Grayscale).</li>
        <li>Apply <strong>K-Means Clustering</strong> to segment foreground from background.</li>
        <li>Use <strong>Watershed Algorithm</strong> to refine object boundaries.</li>
        <li>Apply <strong>Graph Cut (GrabCut)</strong> to extract the final foreground mask.</li>
        <li>Save the final image with a transparent background.</li>
    </ol>
    <h2>How to Run</h2>
    <pre>
    git clone https://github.com/yourusername/Background-Removal-Without-ML.git
    cd Background-Removal-Without-ML
    pip install opencv-python numpy matplotlib
    python background_removal.py --input path/to/image.jpg --output output.png
    </pre>
    <p>Enjoy fast and efficient background removal without deep learning!</p>
</body>
</html>
