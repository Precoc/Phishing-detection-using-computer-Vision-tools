Phishing attacks remain among the most prevalent and dangerous forms of cybercrime in the digital age. These attacks exploit user trust by creating fraudulent websites that visually mimic legitimate ones, tricking users into disclosing sensitive information such as login credentials, financial data, and personal records. According to recent cybersecurity reports, millions of phishing attempts occur daily, causing billions of dollars in financial losses worldwide.

Traditional phishing detection systems primarily relied on textual cues, URL inspection, domain blacklists, and rule-based heuristics. However, modern phishing techniques have evolved to circumvent these methods by embedding malicious content within images, hiding elements behind scripts, using dynamically generated URLs, and employing sophisticated visual obfuscation techniques. Attackers increasingly create visually identical replicas of legitimate websites, making it difficult for both users and conventional detection systems to distinguish authentic domains from fraudulent ones.

This challenge has led to a growing interest in leveraging computer vision - a field within artificial intelligence that enables machines to interpret and understand visual data - for detecting phishing attacks through website screenshot analysis. Unlike conventional text-based methods, visual-based approaches can assess the structural and semantic layout of a webpage, offering a more robust defense against deceptive attacks.

Figure 1.1 below illustrates the typical phishing attack process:

[Insert Figure 1.1: Overview of Phishing Attack Process]

*Caption: Figure 1.1 - Overview of Phishing Attack Process showing how users are redirected from legitimate websites to fake phishing sites*

1.3 Objectives of the Seminar
The primary objectives of this seminar work are as follows:

To develop a computer vision-based framework for detecting phishing websites through screenshot analysis.

To implement and compare multiple feature extraction techniques including ORB (Oriented FAST and Rotated BRIEF), HOG (Histogram of Oriented Gradients), and LBP (Local Binary Patterns) for visual similarity assessment.

To preprocess website screenshots using noise removal, contrast enhancement, and size normalization for improved feature extraction.

To establish a similarity threshold that effectively distinguishes legitimate websites from phishing attempts.

To evaluate the effectiveness of visual-based phishing detection compared to traditional methods.

1.4 Brief Overview of the Approach or Methodology
The methodology employed in this seminar work consists of several key stages:

Dataset Collection: A dataset of website screenshots was collected, comprising both legitimate and known phishing sites. The dataset was organized into folders for systematic analysis.

Image Preprocessing: Each screenshot underwent preprocessing including resizing to 800x600 pixels, noise removal using fastNlMeansDenoisingColored, and contrast enhancement using CLAHE (Contrast Limited Adaptive Histogram Equalization).

Feature Extraction: Multiple visual features were extracted from each image:

ORB features for keypoint detection

HOG features for structural pattern analysis

LBP features for texture analysis

Color histograms for color distribution comparison

Similarity Analysis: Pairwise comparison of images was performed using four similarity metrics: Structural Similarity Index (SSIM), feature matching scores, color histogram correlation, and HOG similarity.

Classification: A similarity threshold of 0.4 was established to classify image pairs as potentially legitimate or potentially phishing.
