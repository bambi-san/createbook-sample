FROM node:15.5.1-stretch-slim

ENV TEXTLINT_VERSION=11.9.0

RUN npm install -g textlint \
    && npm install -g \
       textlint-plugin-review \
       textlint-rule-prh \
       textlint-rule-preset-ja-technical-writing \
       textlint-rule-preset-ja-spacing \
       textlint-filter-rule-comments
WORKDIR /work

CMD ["textlint" , "--config" , "/.textlintrc"]
