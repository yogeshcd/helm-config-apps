#docker build -t val418orant/wishlist:latest .
#docker push val418orant/wishlist:latest

FROM python:3
COPY . .
RUN pip install flask flask_cors
CMD ["python","index.py"]