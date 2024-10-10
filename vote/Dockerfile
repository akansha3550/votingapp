# Step 1: Use an official Python base image
FROM python:3.8-slim

# Step 2: Set the working directory inside the container
WORKDIR /app

# Step 3: Copy the source code to the container's working directory
COPY . .

# Step 4: Install dependencies listed in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Step 5: Expose the port the application will run on
EXPOSE 80

# Step 6: Define the command to run your app
CMD ["python", "app.py"]

