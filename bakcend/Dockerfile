FROM python:3.8
RUN apt-get update && apt-get install -y git
RUN git clone https://gitlab.com/redacre/test-project.git
RUN pip install -r test-project/api/requirements.txt
CMD ["python", "test-project/api/app.py"]
EXPOSE 5000 3000 80 443