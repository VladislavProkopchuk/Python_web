FROM python:3.9

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
COPY ./stocks_products ./site
WORKDIR /site
RUN pip3 install -r requirements.txt
EXPOSE 8000
ENV MyENV=Default
WORKDIR site

