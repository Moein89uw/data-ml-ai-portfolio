# Data, ML, and AI Portfolio

A collection of projects spanning data analytics, classical machine learning, deep learning, natural language processing, and generative AI. Each project lives in its own repository with code, tests, sample data, and documentation that explains the problem, approach, and results.

## About me

I am Moein Khaloei, a data and ML practitioner working across the analytics-to-deep-learning spectrum. My focus is on building reproducible, honest pipelines: code that runs end-to-end with tests, clear documentation of methodology, and results presented with appropriate caveats.

## Featured projects

### Machine learning

**[Bike Rental Demand Forecasting](https://github.com/Moein89uw/bike-rental-demand-forecasting-ml)**
Hourly demand forecasting on 8,760 records using scikit-learn `Pipeline` and `ColumnTransformer` to prevent data leakage. Compares five regression models with cross-validation and selects Polynomial Ridge (test R² = 0.62, MAE = 288). Includes permutation importance on raw features for interpretability.

**[Amazon Product Review NLP/ML](https://github.com/Moein89uw/amazon-product-review-nlp-ml)**
Combined NLP and ML pipeline on Amazon product reviews. TF-IDF for review text combined with numeric and categorical features through `ColumnTransformer`. Includes both rating regression and sentiment classification with honest acknowledgment of class imbalance and an optional deep learning extension path.

**[Home Loan Default Prediction (Deep Learning)](https://github.com/Moein89uw/home-loan-default-prediction-deep-learning)**
Binary classification on imbalanced loan default data with Keras. Uses ROC AUC, sensitivity/specificity, and Youden's J statistic for threshold selection. Includes a lightweight scikit-learn baseline for comparison and reproducibility.

### Natural language processing

**[Banking Complaints NLP Triage](https://github.com/Moein89uw/banking-complaints-nlp-triage)**
Department routing and sentiment-based triage of customer banking complaints. TF-IDF + Logistic Regression with auto-adjusting `min_df`/`max_df` for varying dataset sizes. Includes VADER sentiment and a triage rule that combines department prediction with negative-sentiment scoring.

**[TripAdvisor Review Sentiment + Topic Modeling](https://github.com/Moein89uw/tripadvisor-review-sentiment-topic-modeling)**
Hotel review sentiment classification with multiple models and NMF topic modeling. Includes a CLI prediction tool and lightweight optional transformer extension.

### Deep learning

**[Multimodal Deep Learning Capstone](https://github.com/Moein89uw/deep-learning-multimodal-capstone)**
Four deep learning tasks in one repository: tabular churn classification, face-mask image classification with transfer learning, sentiment classification with LSTM, and dental image denoising with an autoencoder. TensorFlow is lazy-loaded so tests run in any environment.

### Data analytics

**[AAL Apparel Sales Analysis](https://github.com/Moein89uw/aal-apparel-sales-analysis)**
Descriptive sales analytics for an Australian apparel chain. Breakdowns by state, demographic group, and time period with explicit recommendations.

**[Rolling Stones Spotify Song Clustering](https://github.com/Moein89uw/rolling-stones-spotify-song-clustering)**
Unsupervised clustering of the Rolling Stones discography using Spotify audio features. PCA dimensionality reduction, silhouette and elbow analysis for choosing cluster count, and album-level recommendations.

**[BikeEase Rental Analytics](https://github.com/Moein89uw/bikeease-rental-analytics)**
Exploratory analysis of hourly bike rental demand. Weather, seasonality, holiday, and operational-day breakdowns with summary tables and figures.

### Generative AI

**[BikeEase Generative AI Ad Generator](https://github.com/Moein89uw/bikeease-generative-ai-ad-generator)**
Ad copy generation system with a quality-scoring rubric covering relevance, promotion, call-to-action, tone, and structure. Ships with a deterministic demo engine and an optional Hugging Face model path.

**[Nestle HR Policy RAG Chatbot](https://github.com/Moein89uw/nestle-hr-policy-rag-chatbot)**
Retrieval-augmented question answering over HR policy text. TF-IDF retrieval as the local baseline, optional OpenAI generation, and a Gradio chatbot interface.

## How these projects are organized

Each repository follows a consistent structure:

- `src/` — reusable Python package code
- `scripts/` — entry-point scripts for running the pipeline
- `tests/` — pytest test suite
- `data/sample/` — small sanitized samples for tests and demos (when applicable)
- `data/raw/` — local-only location for full datasets (gitignored when applicable)
- `notebooks/` — analysis notebooks
- `outputs/` — generated reports, figures, and model artifacts
- `docs/` — project briefs and data dictionaries
- `requirements.txt` — pinned dependency list
- `pyproject.toml` — package metadata (in projects that use a src-layout package)

All projects include a README with installation instructions, methodology, and results. Tests are included for the core data and modeling logic.

## License

Individual project repositories are released under the MIT License unless otherwise noted.
