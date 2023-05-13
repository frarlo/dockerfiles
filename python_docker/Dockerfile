
FROM python:3
RUN mkdir /mnt/output_python
COPY pepe.py /mnt/output_python
ENTRYPOINT ["python", "pepe.py"]

# Build
docker build -t pepe_py .

# Run
docker run --name hellopepe --rm --mount type=bind,src="$(pwd)",dst="/mnt/output_python" pepe_py
