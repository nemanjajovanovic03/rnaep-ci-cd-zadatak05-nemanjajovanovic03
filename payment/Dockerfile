FROM python:3.10-slim

WORKDIR /app

# Kopiramo requirements.txt iz payment foldera u kontejner i instaliramo zavisnosti
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Kopiramo sav preostali kod iz payment foldera u kontejner
COPY . .

# Pokrećemo main.py koji se nalazi u payment folderu
CMD ["python", "main.py"]
