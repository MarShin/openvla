FROM runpod/pytorch:2.2.0-py3.10-cuda12.1.1-devel-ubuntu22.04@sha256:75bf115d87ee3813f8026fed3e11bae3bf68bfd789a9566878735245b723ef8b

# Install dependencies
RUN pip install git+https://github.com/openvla/openvla

# Install Flash-Attention
RUN pip install packaging ninja
RUN pip install "flash-attn==2.5.5" --no-build-isolation

# Set Python path
ENV PYTHONPATH="/workspaces/openvla"
