# Plant Disease Classification: Comparing ML Algorithms

A 10-week summer research project for high school students.

Title: Comparing Classical Machine Learning and Deep Learning Models for Plant Leaf Disease Classification on the PlantVillage Dataset.

Research question: How do classical ML algorithms (e.g. SVM, Random Forest, XGBoost) compare with deep learning models (CNN, transfer learning) for classifying plant leaf diseases from images, in terms of accuracy, training time, and model size?

## How to start

1. Open `plant_disease_classification.ipynb` -- or launch it directly in Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/VietNguyen705/plant-disease-highschool/blob/main/plant_disease_classification.ipynb)
2. Switch the runtime to GPU (Runtime -> Change runtime type -> T4 GPU).
3. Fill in every TODO cell from top to bottom.

Ask your instructor if stuck.

## 4 Big Steps

1. **Setup + Download** -- Set up Colab/Drive/GitHub, download the PlantVillage dataset, explore the folder structure and view sample leaves.
2. **Data Preprocessing** -- Build a balanced sample, split into train/val/test, run EDA, and extract features (color, texture, shape) for classical ML plus an image pipeline for deep learning.
3. **Training & Evaluation** -- Train and compare many algorithms: classical ML (Logistic Regression, KNN, Decision Tree, Naive Bayes, SVM, Random Forest, XGBoost) and deep learning (CNN from scratch, MobileNetV2, ResNet50, EfficientNet), then consolidate metrics and error analysis.
4. **Write Report** -- Draft the paper, polish figures, build a prediction demo, and prepare the poster and presentation.

## 10-Week Plan

<table>
  <thead>
    <tr><th>Step</th><th>Week</th><th>Tasks</th></tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2"><b>Setup + Download</b></td>
      <td>1</td>
      <td>Learn ML basics, image classification, and the plant disease problem. Set up Python + Colab + GitHub. Download PlantVillage (color) and view sample leaves</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Explore folder structure. Count images per class. Understand the 38 classes across 14 crops</td>
    </tr>
    <tr>
      <td rowspan="2"><b>Data Preprocessing</b></td>
      <td>3</td>
      <td>Build a balanced ~150 images/class sample. Split into train/val/test. EDA: class counts, image sizes, color distributions</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Extract classical-ML features (color histograms, GLCM/LBP texture, shape). Build the deep-learning image pipeline + augmentation. Save reusable feature tables</td>
    </tr>
    <tr>
      <td rowspan="4"><b>Training &amp; Evaluation</b></td>
      <td>5</td>
      <td>Classical round 1: Logistic Regression, KNN, Decision Tree, Naive Bayes. Record accuracy and confusion matrices</td>
    </tr>
    <tr>
      <td>6</td>
      <td>Classical round 2: SVM (linear/RBF), Random Forest, XGBoost. Try hyperparameter variations</td>
    </tr>
    <tr>
      <td>7</td>
      <td>Train a CNN from scratch on Colab GPU. Plot training curves</td>
    </tr>
    <tr>
      <td>8</td>
      <td>Transfer learning: MobileNetV2, ResNet50, EfficientNet. Compare all models (accuracy, F1, training time, model size) + error analysis</td>
    </tr>
    <tr>
      <td rowspan="2"><b>Write Report</b></td>
      <td>9</td>
      <td>Draft the report (intro, dataset, methods, results, discussion). Build a prediction demo (upload a leaf -&gt; predicted disease)</td>
    </tr>
    <tr>
      <td>10</td>
      <td>Final paper, poster, presentation. Discuss limitations and real-world use</td>
    </tr>
  </tbody>
</table>

## Algorithm Variety

- **Classical ML:** Logistic Regression, KNN, Decision Tree, Naive Bayes, SVM (linear & RBF), Random Forest, XGBoost -- each with hyperparameter variations.
- **Deep learning:** CNN from scratch, MobileNetV2, ResNet50, EfficientNet (transfer learning) + data-augmentation variants.

## Dataset

- **PlantVillage** -- ~54,000 leaf images, 38 classes across 14 crops (Apple, Cherry, Corn, Grape, Peach, Pepper, Potato, Strawberry, Tomato, and more), each crop with a healthy class plus disease classes. We use a balanced ~150 images/class sample (~5,700 images).
- GitHub source: https://github.com/spMohanty/PlantVillage-Dataset (use the `raw/color` images).
