# speedtest_http

Visualize data generated by
[speedtest-cli](https://github.com/sivel/speedtest-cli) in a web app
powered by [Plotly](https://plot.ly/python/)


[![Latest Version](https://img.shields.io/pypi/v/speedtest-http.svg)](https://pypi.python.org/pypi/speedtest-http/)
[![Travis](https://img.shields.io/travis/shuntingyard/speedtest-http.svg)](https://pypi.python.org/pypi/speedtest-http/)
[![License](https://img.shields.io/pypi/l/speedtest-http.svg)](http://github.com/shuntingyard/speedtest_http/blob/master/LICENSE.txt)
[![Docker Image](https://img.shields.io/docker/cloud/build/shuntingyard/speedtest_http.svg)](https://cloud.docker.com/repository/docker/shuntingyard/speedtest_http/)
[![Versions](https://img.shields.io/pypi/pyversions/speedtest-http.svg)](https://pypi.python.org/pypi/speedtest-http/)

## Screenshots

### Desktop

![Desktop Heatmap](static/Heatmap30.png)

### Android

![Android Lineplot](static/LineplotTodayAndroid.png)

## Install and run

### dockerhub

Get up and running instantly, with a speedtest.csv file in your home dir and
logs written to stdout.

```
   # Please adapt details (container timezone, sitename) to your needs.

   docker run -ti -p 80:5000 -v ~:/root -e FLASK_DEBUG=1 -e "TZ=EST" \
      -e "INFILE=/root/speedtest.csv" -e "SITENAME=my provider" \
      shuntingyard/speedtest_http
```

## README.rst

Please continue reading [here](https://pypi.org/project/speedtest-http/).
