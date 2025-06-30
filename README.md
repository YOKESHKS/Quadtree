🧠 Quadtree Image Representation and Visualization
This project demonstrates how to recursively split an image using the Quadtree data structure. The main goal is to divide an image into quadrants based on color similarity and visualize how it is reconstructed at various levels of the tree.


🧾 Features
📐 Image split into 4 quadrants recursively (North-West, North-East, South-West, South-East)

🎨 Mean color computation for each quadrant

🌳 QuadTree data structure with adaptive decomposition

🔁 Image reconstruction at different tree levels

🖼️ Matplotlib visualization of each level's output

🔧 Requirements
Install dependencies using:


pip install matplotlib numpy
📁 Project Structure

Quadtree/
│
├── Untitled-1.ipynb         # Main code notebook
├── IMG_*.jpg                # Input image (can be changed)
├── README.md                # Project documentation
└── requirements.txt         # Required libraries
🚀 How It Works
1. Image Splitting
Splits the image into 4 quadrants using NumPy's array_split.

2. Mean Calculation
Computes the average RGB value of each quadrant.

3. Recursive Insertion
Builds the Quadtree recursively. If a region is not uniform, it's split further.

4. Image Reconstruction
Generates a blurred/abstracted version of the image based on the desired Quadtree depth.

🧠 Sample Code Snippet

quadtree = QuadTree()
quadtree.insert(img)

plt.imshow(quadtree.get_image(3))
plt.show()
📊 Output Explanation
Level	Description
1	Entire image is divided into 4 blocks
3	Finer details begin to appear
7	Image starts to resemble the original
10	High resolution with more accurate color regions

To install dependencies, use:


pip install -r requirements.txt

📌 Use Cases
Image Compression

Spatial Indexing

Efficient Image Representation

AI/ML Preprocessing for Satellite or Medical Images

📬 Author
👨‍💻 Yokesh K. S.

📝 License
This project is open-source and available under the MIT License.

📎 To Do
 Add GUI interface for uploading image

 Add option to export compressed images

 Optimize performance for larger images

