
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
    <div class="container">
        <div class="column">
            <h3>Input Images</h3>
            <img src="input1.jpg" alt="Input Image 1">
            <img src="input2.jpg" alt="Input Image 2">
        </div>
        <div class="column">
            <h3>Output Images</h3>
            <img src="output1.png" alt="Output Image 1">
            <img src="output2.png" alt="Output Image 2">
        </div>
    </div>

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
    # Clone the repository
    git clone https://github.com/yourusername/Background-Removal-Without-ML.git
    cd Background-Removal-Without-ML
    
    # Install dependencies
    pip install opencv-python numpy matplotlib

    # Run the script
    python background_removal.py --input path/to/image.jpg --output output.png
    </pre>

    <p>Enjoy fast and efficient background removal without deep learning! 🚀</p>
</body>
</html>
