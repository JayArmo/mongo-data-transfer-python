# MongoDB Data Transfer Python Script

![Python](https://img.shields.io/badge/Python3-blue)
![License](https://img.shields.io/badge/License-MIT-green)

## Overview

This Python script facilitates the seamless transfer of data between MongoDB databases. It connects to a source MongoDB database, retrieves user information, and transfers it to a specified destination database. The script ensures efficient and secure migration of data, making it a valuable tool for managing MongoDB databases in various applications.

## Features

- **Flexible Configuration**: Easily customize source and destination MongoDB connection details.
- **User Data Transfer**: Transfer user information, ensuring data consistency between databases.
- **Error Handling**: Robust error handling to manage exceptions during the data transfer process.

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/JayArmo/mongo-data-transfer-python
   ```

2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage

1. Configure MongoDB URLs in `main.py`.
   ```python
   SOURCE_DB_URL = ""
   DESTINATION_DB_URL = ""

   source_client = MongoClient(SOURCE_DB_URL)
   source_db = source_client['My_DB']
   source_collection = source_db['users']

   destination_client = MongoClient(DESTINATION_DB_URL)
   destination_db = destination_client['My_DB']
   destination_collection = destination_db['users']
   ```
2. Run the script:
   ```
   python main.py
   ```

## License

This project is licensed under the [MIT License](LICENSE) - see the [LICENSE](LICENSE) file for details.

## Contribution

Contributions are welcome! Please fork the repository and submit a pull request.

## Acknowledgements

- [pymongo](https://pypi.org/project/pymongo/): MongoDB driver for Python.

## Support

For any questions or issues, please [open an issue](https://github.com/JayArmo/mongo-data-transfer-python/issues).
