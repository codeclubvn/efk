FROM fluent/fluentd:v1.16-debian-1

# Chuyển quyền root để cài đặt plugin
USER root

RUN gem install elasticsearch -v 8.8.0

RUN ["gem", "install", "fluent-plugin-elasticsearch", "--no-document", "--version", "5.3.0"]

# Quay lại quyền user mặc định của Fluentd
USER fluent
