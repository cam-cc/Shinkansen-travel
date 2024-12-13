# 🚅 Shinkansen Passenger Experience Predictor
## Top 5 Finalist - University Hackathon 2023

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/downloads/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-Latest-orange.svg)](https://scikit-learn.org/stable/)
[![Accuracy](https://img.shields.io/badge/Accuracy-95%25-success.svg)](#results)

## Overview
An advanced machine learning solution for predicting passenger satisfaction on Japan's Shinkansen Bullet Train system. This project achieved 95% accuracy in predicting customer satisfaction based on travel and survey data, earning a top 5 placement in the 2023 University Hackathon.

## Project Structure
```
├── data/
│   ├── train/
│   │   ├── travel_data.csv
│   │   └── survey_data.csv
│   └── test/
├── models/
├── notebooks/
└── src/
```

## Dataset Details
The analysis utilizes two primary datasets:
- **Travel Data**: Passenger and train-specific attributes
- **Survey Data**: Aggregated post-service experience metrics

Target Variable:
- `Overall_Experience`: Binary classification
  - 1: Satisfied
  - 0: Not Satisfied

## Model Performance
- **Best Model**: AdaBoost Classifier
- **Accuracy**: 95%
- **Training Set Size**: 35,602 entries
- **Features Used**: Travel metrics + Survey responses

## Implementation

### Requirements
```bash
pandas==1.5.3
scikit-learn==1.2.2
numpy==1.23.5
scipy==1.10.1
```

### Quick Start
1. **Clone the repository**
```bash
git clone https://github.com/yourusername/shinkansen-satisfaction.git
cd shinkansen-satisfaction
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Run the model**
```bash
python src/train_model.py
```

## Model Details

### AdaBoost Configuration
```python
# Default Configuration (95% accuracy)
AdaBoostClassifier(
    learning_rate=0.1,
    n_estimators=100
)
```

## Output Format
- CSV file with 35,602 predictions
- Columns: ID, Overall_Experience (0/1)

## Evaluation Metrics
- Primary Metric: Accuracy Score
- Cross-validation implemented
- Confusion matrix analysis available

## Future Improvements
- [ ] Feature importance analysis
- [ ] Hyperparameter optimization
- [ ] Ensemble with other models
- [ ] Real-time prediction API

## Contributors
<table>
  <tr>
    <td align="center">
      <a href="https://github.com/yourusername">
        <sub><b>Your Name</b></sub>
      </a>
    </td>
  </tr>
</table>

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Competition organizers
- Faculty mentors
- Dataset providers

---
<p align="center">Made for University Hackathon 2023</p>
```
