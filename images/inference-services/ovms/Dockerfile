ARG BASE_PREDICTOR_IMAGE=ghcr.io/fuseml/base-predictor
FROM $BASE_PREDICTOR_IMAGE

ENV FUSEML_ENV_WORKFLOW_NAMESPACE fuseml-workloads
ENV FUSEML_ENV_WORKFLOW_NAME ""
ENV AWS_ACCESS_KEY_ID ""
ENV AWS_SECRET_ACCESS_KEY ""
ENV S3_ENDPOINT ""
ENV FUSEML_MODEL ""
ENV FUSEML_MODEL_NAME default
ENV FUSEML_OVMS_IMAGE_TAG "2021.4.1"

RUN mkdir /opt/openvino/
COPY run.sh /usr/local/bin/run
COPY templates /opt/openvino/templates

CMD [ "run" ]
