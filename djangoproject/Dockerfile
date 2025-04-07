FROM python:3.9

# Set the working directory
WORKDIR /var/www/app


# Install dependencies
RUN pip install Django
RUN pip install psycopg2

# Copy the entire Django project to the working directory
COPY . .

# Expose port
EXPOSE 80

# Command to run the application
CMD ["python3", "manage.py", "runserver", "0.0.0.0:80"]

