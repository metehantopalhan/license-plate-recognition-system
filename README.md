# License Plate Recognition system:(LRR)
##### -license plate recognition system will work with camera to identify the plate number of the car that tries to enter the parking lot, and also check if the car allowed/not allowed to enter by checking the DB of the system.

##### -We have used various approaches to achieve a high accuracy depending on the provided data to detect, segment plate characters, classify these characters and check the DB to allow/not allow the car to enter parking lot.

## Setup

1. Install Python 3 and clone this repository.
2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Configure database credentials using environment variables:
   - `DB_USER` – database user (default `postgres`)
   - `DB_PASSWORD` – **required**, the database password
   - `DB_HOST` – database host (default `127.0.0.1`)
   - `DB_PORT` – database port (default `5432`)
   - `DB_NAME` – database name (default `plates`)
4. Run the API server:
   ```bash
   python py_files/API.py
   ```

The service exposes a `/Process` endpoint that accepts an image file via POST request and returns the recognition result.



