FROM python:3.9-alpine

# Install necessary system packages for Gunicorn & Python dependencies
RUN apk update && apk add --no-cache gcc musl-dev libffi-dev

# Create app directory
RUN mkdir -p /var/flaskapp
WORKDIR /var/flaskapp

# Copy app files
COPY . .

# Install Python dependencies
RUN pip3 install --no-cache-dir -r requirements.txt

# Expose Flask port
EXPOSE 5000

# Use Gunicorn to run the Flask app
CMD ["gunicorn", "--bind", "0.0.0.0:5000", "app:app"]
