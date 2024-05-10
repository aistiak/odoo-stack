FROM odoo:latest
WORKDIR /app

COPY . .

RUN pip install setuptools wheel
RUN pip install -r requirements.txt

CMD ["python", "odoo-bin", "-r", "dbuser", "-w", "dbpassword", "--addons-path=/mnt/extra-addons", "-d", "mydb"]
