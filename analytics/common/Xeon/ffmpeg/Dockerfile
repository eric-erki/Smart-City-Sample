# smtc_analytics_common_xeon_ffmpeg

From openvisualcloud/xeon-ubuntu1804-analytics-ffmpeg:19.11
RUN DEBIAN_FRONTEND=noninteractive apt-get update -qq && apt-get install -qq python3-gst-1.0 python3-jsonschema && rm -rf /var/lib/apt/lists/*

COPY app /home/
COPY *.py /home/