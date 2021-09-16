FROM nginx:alpine

LABEL maintainer:"JT" version:"2021.01" description:"My nginx homepage in docker"

ENV AUTHOR JT
ENV VERSION 2021.01
ENV TITLE "Nginx in Docker homepage" 

ADD startbootstrap-freelancer-gh-pages/ /usr/share/nginx/html/

RUN sed -i s/--AUTHOR--/"$AUTHOR"/g /usr/share/nginx/html/index.html \
 && sed -i s/--VERSION--/"$VERSION"/g /usr/share/nginx/html/index.html \ 
 && sed -i s/--TITLE--/"$TITLE"/g /usr/share/nginx/html/index.html

