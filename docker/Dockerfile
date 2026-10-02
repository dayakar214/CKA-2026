FROM python:3.9

WORKDIR /app
ENV APP_ENV=production.
RUN pip install flask gunicorn  
COPY . .
RUN useradd -m xdeploy  
USER xdeploy
EXPOSE 5000
CMD ["python", "app.py"]



