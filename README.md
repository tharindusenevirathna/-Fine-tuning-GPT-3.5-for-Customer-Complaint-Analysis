
# Fine-tuning GPT-3.5 for Customer Complaint Analysis 

This project fine-tunes the GPT-3.5 model using the OpenAI API to analyze customer complaints for a telecommunications company. The model extracts critical details, including the topic, problem, and a customer dissatisfaction index ranging from 0 to 100. This helps company to better understand customer issues and improve overall service quality.

## Main Objective of the Project

The primary goal of this project is to fine-tune GPT-3.5 to accurately analyze and extract structured information from unstructured customer complaints. By automating the extraction of the topic, problem, and customer dissatisfaction index, company can identify and prioritize service issues, helping improve customer satisfaction.

## Features

- Extracts key details from customer complaints: topic, problem, and dissatisfaction index
- Utilizes OpenAI’s GPT-3.5 for fine-tuning
- Prepares training data for model fine-tuning
- Deploys the fine-tuned model to analyze real-time complaints
- Provides insights to enhance customer service

## Technologies Used

- **OpenAI API (GPT-3.5)**: For model fine-tuning and real-time inference
- **Python**: Core programming language for data processing and integration
- **Pandas**: For handling and manipulating customer complaints data
- **dotenv**: For managing environment variables securely
- **JSON**: For structuring the fine-tuning data

## Project Structure

```
├── fine_tuning_data.json   # Prepared dataset in JSON format for model training
├── prepare_data.py         # Script to convert customer complaints to JSON format
├── fine_tune_model.py      # Script to fine-tune the GPT-3.5 model
├── evaluate_model.py       # Script to evaluate the fine-tuned model
├── deploy_model.py         # Script to deploy and test the fine-tuned model
├── .env                    # Environment file to store OpenAI API key
└── README.md               # Project documentation
```



## How to Use

- **Fine-tune the model**: The `fine_tune_model.py` script uploads the prepared training data to the OpenAI API and fine-tunes GPT-3.5 for customer complaint analysis.
- **Evaluate the model**: The `evaluate_model.py` script tracks metrics such as training loss and accuracy during the fine-tuning process.
- **Deploy and test**: The `deploy_model.py` script allows you to input new complaints and get extracted topics, problems, and dissatisfaction index in real time.

